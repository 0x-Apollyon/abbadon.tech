---
title: "Provable, Fair Randomness in Online Gambling"
description: "A walkthrough on creating a provably fair and random online gambling game (Mines) using Python, covering cryptographic seed generation, client-server seed combination, and client-side verification."
author: "0xApollyon"
tags: [provably-fair, online-gambling, randomness, cryptography, python, game-development, verification]
category: "Security Research"
keywords: ["provably fair gambling", "online gambling randomness", "mines game", "client seed server seed", "SHA256 verification", "cryptographic randomness", "provable fairness"]
source_url: "https://abbadon.tech/blog/"
---

# Provable, Fair Randomness in Online Gambling

## Introduction

In recent years, online gambling platforms such as Stake have experienced significant growth, generating billions of dollars in profit. This raises a critical question: **How can we be certain that these online platforms are not rigging the games against their users?**

In this writeup, we will explore the creation of a provably fair and random game similar to Mines, which is one of the most popular gambling games available.

All the code in this writeup will be in Python, so a basic understanding of Python would be helpful.

---

## Requirements

Our implementation has three key requirements:

- The position of the mines should be random
- The user should not be able to determine the position of the mines with any probability greater than what would occur by random chance
- The user should be able to see the position of the mines and determine whether the game was fair or not once it ends

---

## Code Implementation

We'll be designing a game of Mines where the grid is of size n*n and has m mines. For this example, we'll consider a grid of size 3*3 with 1 mine, but you can tweak these parameters as needed.

```python
# Game Configuration
square_size = 3
number_of_mines = 1
number_of_tiles = square_size * square_size
number_of_gems = number_of_tiles - number_of_mines

if number_of_tiles < number_of_mines:
    print("Number of tiles can't be less than number of mines")
    quit()

# Create game layout
game_layout = []

# Add mines
for i in range(number_of_mines):
    game_layout.append(1)

# Add gems
for i in range(number_of_gems):
    game_layout.append(0)

# game_layout is an array with 1s (mines) and 0s (gems)
```

---

## Adding Randomness

We'll use Python's random module and the os module for generating cryptographically secure randomness:

```python
import random
import os

# Generate cryptographically random server seed
server_seed = os.urandom(32)
random.seed(server_seed)
random.shuffle(game_layout)
```

---

## Enhanced Randomness with Client Seed

To prevent manipulation, we incorporate a client-side seed:

```python
import random
import os
import hashlib

# Generate server seed and its hash
server_seed = hashlib.sha256(os.urandom(32)).hexdigest()
server_seed_hashed = hashlib.sha256(server_seed.encode()).hexdigest()

# Display server seed hash
print(f"The current server seed hash is {server_seed_hashed}")

# Get client seed
client_seed = input("Enter client seed: ").strip()
client_seed_hashed = hashlib.sha256(client_seed.encode()).hexdigest()

# Create final seed
final_seed = client_seed_hashed + server_seed

# Shuffle game layout
random.seed(final_seed)
random.shuffle(game_layout)
```

---

## Game Logic and State Management

```python
# Convert 1D layout to 2D grid
square_layout = []
square_row = []
for j, i in enumerate(game_layout):
    square_row.append(i)
    if (j+1) % square_size == 0:
        square_layout.append(square_row)
        square_row = []

# Initialize game state
mine_struck = False 
game_state = []
for i in range(square_size):
    row = [0] * square_size
    game_state.append(row)

# Game loop
while not mine_struck:
    # Display current game board
    print("\n")
    for i, row in enumerate(square_layout):
        for j, element in enumerate(row):
            if game_state[i][j] == 0:
                print(f"  [{i+1} , {j+1}]  ", end="")
            else:
                print("     *     ", end="")
        print("")
    print("\n")

    # Get user input
    coords = input("Select the tile with its numbers split with a comma or quit to end the game: ").strip()
    
    if coords != "quit":
        coords = coords.split(",")
        first_coord = int(coords[0])
        second_coord = int(coords[1])

        # Check if mine is struck
        if square_layout[first_coord-1][second_coord-1] == 1:
            print("You hit the mine. BOOM !!")
            print(f"Client seed for verification: {server_seed}")
            mine_struck = True
        else:
            game_state[first_coord-1][second_coord-1] = 1
    else:
        print("Game ended")
        print(f"Client seed for verification: {server_seed}")
        mine_struck = True
```

---

## Client-Side Verification

```python
# Verification Script
square_size = 3
number_of_mines = 1
number_of_tiles = square_size * square_size
number_of_gems = number_of_tiles - number_of_mines

# Create game layout
game_layout = []
for i in range(number_of_mines):
    game_layout.append(1)
for i in range(number_of_gems):
    game_layout.append(0)

import hashlib
import random

# Get verification inputs
client_input = input("What was the client input: ").strip()
server_seed = input("What was the final revealed server seed: ").strip()
server_seed_hash = input("What was the initially revealed server seed hash: ").strip()

# Verify seed and hash
client_input_hashed = hashlib.sha256(client_input.encode()).hexdigest()
final_seed = client_input_hashed + server_seed

# Check seed integrity
if hashlib.sha256(server_seed.encode()).hexdigest() == server_seed_hash:
    print("Server Seed Hash verified. The game was provably fair.")
else:
    print("Server Seed Hash verification failed, the game wasn't fair.")

# Reproduce game layout
random.seed(final_seed)
random.shuffle(game_layout)

# Display final layout
for j, i in enumerate(game_layout):
    if i == 0:
        print("   GEM   ", end="")
    else:
        print("   MINE  ", end="")

    if (j+1) % square_size == 0:
        print()
```

---

## Conclusion

This is a fundamental example using the game Mines, but the principles of provable randomness can be applied to all types of gambling games.

Full code available at: [github.com/0x-Apollyon/Provable-Randomness](https://github.com/0x-Apollyon/Provable-Randomness)