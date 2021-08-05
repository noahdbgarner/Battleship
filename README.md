# Battleship (OOP Python Version)

## 1. Introduction

### Description
This program plays the classic game Battleship. It was built to be scalable with respect to grid dimensions and ships.
Feel free to add/remove ships or change cols and rows in data.json

### Technologies

* Python version > 3.6 
   - This is required because I make use of annotating variables and functions with type hints

## 2. Design

### 2.1 Files
1. **data.json**
   - contains grid dimension and ship data
2. **grid.py**
   - contains the Grid class
3. **play_battleship.py**
   - contains the driver program
4. **player.py**
   - contains the Player class
5. **ship.py**
    - contains the Ship class

### 2.2 Object Relations
- The driver creates two players
- A player has a grid
- A grid has many ships

## 3. Setup

### Instructions
- In terminal, run `python3 play_battleship.py`

## 4. Approach
- First, I tried solving the problem using a two-dimensional array which I would iterate over to place ships on the board
- After drawing out this solution, I found that it would be more efficient to track ship locations with a list, and shots fired with a dictionary

## 5. Future Improvements
- The computer's coordinate choice could be made more intelligent. One way to do this would be to add a function that checks coordinates within a close area of a damaged ship