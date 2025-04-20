# 🧩 Maze Puzzle Quest

**Maze Puzzle Quest** is an immersive puzzle-adventure game built with Pygame, where the player navigates through a mysterious maze filled with challenging puzzles, foggy areas, and interactive elements like teleporters and traps. The goal? Solve all puzzles, avoid penalties, and escape the maze with the highest score possible.

---

## 🎮 Game Features

- 🧠 **Diverse Puzzle Challenges** – 6 categories of puzzles logic, spatial reasoning, riddles, item use, lateral thinking and exploration.
- 🔄 **Dynamic Maze Behavior** – Revisiting cells affects your score and progression:
  - Visit a cell **twice** → turns yellow and **reduces score**.
  - Visit a cell **three times** → it **blocks permanently** and further reduces score.
- 🌫️ **Foggy Maze Sections** – Players need to find and use a light source to navigate hidden areas.
- 🌀 **Teleporters** – Two teleporters exist in the maze, offering quick traversal… if you can reach them.
- 🧾 **Score & Grading System** – Final scores are graded from S to C based on performance.

---

## 🧩 Puzzle Summary

### 🐉 1. **Three-Headed Dragon (Riddle)**
Face a dragon with three heads. Each head asks a riddle, increasing in difficulty. Solve all to escape the flames, or get burnt!

### 🔥 2. **Matchstick Equation (Lateral Thinking)**
Presented with a faulty equation built using matchsticks, you must move one matchstick to make the equation correct.

### 🚢 3. **Battleship Puzzle (Spatial Reasoning)**
Inspired by the classic game — place all your ships correctly and sink your opponent's fleet on a grid.

### 🎩 4. **Hat Logic Puzzles (Deductive Reasoning)**
Two puzzles involving prisoners guessing hat colors — including the classic line-up puzzle where only logic can save them.

### 💡 5. **Item Use Puzzle (Fog Navigation)**
To pass through the fog, you must gather coins and purchase a light source from a shopkeeper character.

### 🗝️ 6. **Exploration Puzzle (Escape Room Style)**
You encounter a locked door and a mysterious box nearby. Inside is a code and a clue to unlock your path forward.

---

## 🗂️ Project Structure

```
├── main.py                  # Game loop and core logic
├── puzzles_function.py      # Puzzle launching interfaces
├── assets/                  # Fonts, images, icons, puzzle visuals
├── core/
│   └── app.py               # Puzzle mini-game runner logic
├── battleship/              # Battleship-specific puzzle logic
```

---

## 📊 Scoring & Grading

- Player starts with 2000 scores
- Solving puzzles **adds score**
- Moving reduces 10 scores
- Re-entering cells **deducts score**:
  - Second visit: -10 points
  - Third visit: -30 points and path is blocked
- Grading:
  - **S**: ≥ 3750
  - **A**: 3651–3749
  - **B**: 3401–3650
  - **C**: ≤ 3400

---

## 🔊 Audio Feedback

The game includes dynamic sounds for different events:
- Footsteps
- Puzzle success/failure
- Teleportation
- Item collection
- Combat hits & misses (in battleship)

---

## 🚀 Getting Started

1. Make sure you have **Python 3.9+** and **Pygame** installed.
2. Clone the repository:
   ```bash
   git clone https://github.com/yourusername/maze-puzzle-quest.git
   cd maze-puzzle-quest
   ```
3. Run the game:
   ```bash
   python main.py
   ```

---

## 💡 Inspiration

This project combines elements from:
- Classic puzzle games like *Professor Layton* and *The Room*
- Board games like *Battleship*
- Logic riddles and lateral thinking challenges
