# Module I: Introduction to AI and Problem Representation

## 1. Introduction to Artificial Intelligence (AI)
Artificial Intelligence is a branch of computer science that focuses on creating systems capable of performing tasks that normally require human intelligence. These include learning, reasoning, problem-solving, understanding natural language, and perception. The goal of AI is to create machines that can function intelligently and independently.

## 2. Importance of AI
AI has vast applications across industries:
- **Healthcare:** AI algorithms can detect diseases like cancer in medical images.
- **Finance:** Fraud detection systems use machine learning to flag unusual transactions.
- **Transportation:** Autonomous vehicles use AI for navigation and obstacle avoidance.
- **Customer Service:** Chatbots like Siri or Alexa respond to user queries.
- **Manufacturing:** Predictive maintenance uses AI to prevent equipment failure.

## 3. AI Problems
- **Tic Tac Toe Problem:** A 3x3 game where two players alternate marking spaces. AI can use the minimax algorithm to choose the best move.
- **Water Jug Problem:** Given two jugs (e.g., 4L and 3L) and an infinite water supply, measure exactly 2 liters. AI models the problem as a series of states and transitions.

## 4. Application Areas of AI
- **Natural Language Processing (NLP):** Google Translate
- **Robotics:** Self-navigating vacuum cleaners
- **Expert Systems:** Medical diagnosis (MYCIN)
- **Machine Learning:** Spam email filtering
- **Computer Vision:** Facial recognition in social media
- **Speech Recognition:** Voice-to-text in smartphones

## 5. Problem Representations
- **State Space Representation:**  
  E.g., solving a maze. Each position in the maze is a state; moving to another position is an action.

- **Problem Reduction:**  
  E.g., solving the Tower of Hanoi by reducing the problem into moving smaller sets of disks.

- **Production Systems:**  
  Example: IF the light is red THEN stop.

### Characteristics:
- **Deterministic:** Same action always results in the same outcome.
- **Static:** The world does not change while solving.

### Types:
- **Monotonic:** Used in logical deduction.
- **Non-monotonic:** Used when new facts can change conclusions.


# Module II: Heuristic Search Techniques

## 1. AI and Search Process
AI uses search to find optimal or acceptable solutions in large problem spaces. Search algorithms can be:
- **Uninformed:** No additional information (e.g., BFS, DFS)
- **Informed:** Uses heuristics (e.g., A*, Best First Search)

## 2. Uninformed Search Techniques (Brute Force)

### Depth-First Search (DFS):
- **Example:** Navigating a file system directory.
- May go deep without finding a solution.

### Breadth-First Search (BFS):
- **Example:** Finding the shortest path in a grid.
- Guaranteed to find the shortest path but uses more memory.

### Time and Space Complexities:
- **DFS:** Time = O(b^m), Space = O(m)
- **BFS:** Time = O(b^d), Space = O(b^d)

## 3. Heuristic Search Techniques
- **Heuristic:** For the 8-puzzle, the heuristic could be the number of misplaced tiles.
  
- **Hill Climbing:** Choose the move that appears best at the moment.  
  **Example:** Finding max height in terrain navigation.

- **Best First Search:** Uses a priority queue; chooses the path with the lowest cost estimate.

- **A* Algorithm:** Combines path cost (g(n)) + heuristic (h(n)).  
  **Example:** GPS navigation systems.

- **Beam Search:** Keeps top 'k' best paths.  
  **Example:** Speech recognition.

- **AO* Search:** Used in goal trees where goals can be AND/OR nodes.  
  **Example:** AI planning where a task requires multiple sub-tasks.

## 4. Constraint Satisfaction Problems (CSP)
- **Example:** Sudoku puzzle
  - **Variables:** Cells
  - **Domains:** Digits 1-9
  - **Constraints:** No repeated digits in rows, columns, blocks

CSPs are solved using backtracking, forward checking, and heuristics.



# Module III: Game Playing

## 1. AI and Game Playing
Games provide a structured way to test intelligent behavior. Games can be:
- **Deterministic** or **stochastic**
- **Perfect information** (e.g., Chess) or **imperfect information** (e.g., Poker)

## 2. Plausible Move Generator
Generates possible legal moves.  
**Example:** In Chess, a move generator would provide all legal piece movements from the current position.

## 3. Static Evaluation Function
Assigns value to board state without looking ahead.  
**Example:** In Chess, evaluating based on material (piece count) and position.

## 4. Game Playing Strategies

### Minimax Algorithm:
- **Example:** Tic Tac Toe
- AI chooses a move that minimizes the possible loss.

### Alpha-Beta Pruning:
- Prunes unneeded branches.
- **Example:** Reduces time complexity in Chess.

## 5. Problems in Game Playing
- **Combinatorial Explosion:** Too many possible moves (e.g., Go has 10^170 states).
- **Time Constraints:** Limited thinking time in real games.
- **Uncertainty:** Incomplete knowledge of the opponent’s strategy.
