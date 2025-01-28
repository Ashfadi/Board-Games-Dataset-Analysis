# Board Games Dataset Analysis

## Overview
This project involves cleaning, analyzing, and extracting insights from a dataset about board games, sourced from [Kaggle](https://www.kaggle.com/andrewmvd/board-games). The dataset contains information on thousands of board games, including their ratings, player requirements, playtime, and game mechanics. The objective is to explore the dataset using **Pandas** and generate meaningful insights.

---

## Objectives
1. Clean the dataset by handling missing values, invalid data, and inconsistent data types.
2. Perform exploratory data analysis to answer specific questions about board games.
3. Use Python’s Pandas library to manipulate the dataset efficiently without loops or conditional statements.
4. Extract insights related to game complexity, player preferences, and domain-specific trends.

---

## Tools and Technologies
- **Programming Language**: Python
- **Libraries**:
  - `pandas`: For data manipulation and analysis.

---

## Dataset Details
- **Source**: [Kaggle: Board Games Dataset](https://www.kaggle.com/andrewmvd/board-games)
- **Columns**:
  - `ID`: Unique identifier for the game.
  - `Name`: Name of the board game.
  - `Year Published`: Year the game was published.
  - `Min Players` and `Max Players`: Minimum and maximum players required for the game.
  - `Play Time`: Average playtime of the game (in minutes).
  - `Min Age`: Minimum recommended age for players.
  - `Users Rated`: Number of users who rated the game.
  - `Rating Average`: Average rating given to the game by users.
  - `BGG Rank`: BoardGameGeek ranking of the game.
  - `Complexity Average`: Average complexity score of the game.
  - `Owned Users`: Number of users who own the game.
  - `Mechanics` and `Domains`: Lists of game mechanics and domains.

---

## Key Tasks and Insights

### **Task 1: Handle Missing and Invalid Data**
- Identified columns with null values:
  - `ID`, `Year Published`, `Owned Users`, `Mechanics`, and `Domains`.
- Replaced missing values:
  - Used `5000` for missing years and `-1` for missing owned user counts.
- Converted data types for proper analysis.

### **Task 2: Identify Games Published Before 1900**
- Found the number of games published before 1900 (excluding year 0 as it indicates missing data).
- Example Output:
  - Total games published before 1900: **111**
  - Oldest game: **Senet**

### **Task 3: Analyze Popularity by Minimum Players**
- Computed the average ownership for games based on the `Min Players` column.
- Observed that games with fewer minimum players tend to have higher ownership.

### **Task 4: Examine Rating and Complexity**
- Created pivot tables to analyze relationships between `Rating Average` and `Complexity Average`.
- Found a positive correlation:
  - Games with higher complexity tend to have higher ratings.

### **Task 5: Explore Game Domains**
- Used one-hot encoding on the `Domains` column to determine the frequency of each domain type.
- Example Output:
  - Most common domain: **Wargames** (3316 games).
  - Least common domain: **Customizable Games** (297 games).

---

## How to Run

1. **Clone the Repository**:
   ```bash
   git clone https://github.com/<your-username>/Board-Games-Analysis.git
