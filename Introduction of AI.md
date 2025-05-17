## Module I: Introduction to AI and Problem Representation

---

### 1. Introduction to Artificial Intelligence (AI)

**Definition**:  
Artificial Intelligence (AI) is the branch of computer science that aims to create systems that can perform tasks that would normally require human intelligence.

**Importance of AI**:
- Automation of repetitive tasks.
- Decision-making with high accuracy.
- Data analysis and pattern recognition.
- Enhancing user experience (e.g., chatbots, recommendation systems).
- Used in robotics, healthcare, finance, gaming, etc.

---

### 2. AI Problems

AI focuses on solving problems that require reasoning, planning, learning, or decision-making.

#### Examples:

1. **Tic-Tac-Toe Problem**:
   - A simple two-player game.
   - Goal: Build an AI that can play and win or draw.
   - Involves game trees and minimax algorithm.

2. **Water Jug Problem**:
   - Given two jugs with different capacities, find a series of steps to get the desired quantity.
   - Solved using **state space representation**.

---

### 3. Application Areas of AI

- **Expert Systems** – Decision-making in domains like medicine, law.
- **Natural Language Processing (NLP)** – Chatbots, language translation.
- **Robotics** – Autonomous vehicles, industrial robots.
- **Computer Vision** – Face recognition, image classification.
- **Gaming** – AI opponents, game strategies.
- **Healthcare** – Diagnosis, personalized treatment.
- **Finance** – Fraud detection, trading algorithms.

---

### 4. Problem Representation in AI

How a problem is represented plays a key role in designing an AI solution.

#### 4.1 State Space Representation:

- **Definition**: Represents all possible states the system can be in and how transitions between states occur.
- **Components**:
  - Initial state
  - Goal state
  - Operators (actions)
  - Path cost (optional)
- **Example**: Water Jug Problem

#### 4.2 Problem Reduction Representation:

- Breaks a complex problem into smaller sub-problems.
- Uses AND-OR graphs.
- Helps in hierarchical planning and solving.

#### 4.3 Production System:

- Consists of:
  - **Set of rules (productions)**: IF condition THEN action
  - **Working memory**: Current state
  - **Control strategy**: Selects which rule to apply
- Used in expert systems and decision-making.

---

### 5. Characteristics of Production Systems

- **Simplicity**: Easy to modify rules.
- **Modularity**: Each rule is independent.
- **Flexibility**: Can handle new situations by adding new rules.
- **Transparency**: Easy to trace the logic behind actions.

---

### 6. Types of Production Systems

1. **Monotonic**:
   - Application of rules does not prevent the application of other rules in future.
   - Useful in theorem proving.

2. **Non-monotonic**:
   - Application of a rule may prevent the application of another rule.
   - Used in real-time systems.

3. **Deterministic**:
   - Rules produce predictable outcomes.
   - Suitable for well-defined problems.

4. **Non-deterministic**:
   - Multiple rules may be applied; outcomes are uncertain.
   - Used in planning, learning, and search problems.

---

### Summary Table

| **Concept**                | **Key Idea**                                               |
| -------------------------- | ---------------------------------------------------------- |
| AI                         | Making machines simulate human intelligence                |
| Tic-Tac-Toe, Water Jug     | Examples of problem-solving in AI                          |
| Application Areas          | NLP, Robotics, Vision, Healthcare, etc.                    |
| State Space                | States, transitions, goal states                           |
| Problem Reduction          | Divide-and-conquer using sub-problems                      |
| Production System          | Rules + Working memory + Control strategy                  |
| Types of Production System | Monotonic, Non-monotonic, Deterministic, Non-deterministic |

---

## Module II: Heuristic Search Techniques

---

### 1. AI and Search Process

- **AI Problem Solving = Search**  
  AI uses **search** to explore possible solutions in a **state space**.

- **Key Concepts**:
  - **Initial State**: Starting point.
  - **Goal State**: Desired outcome.
  - **Operators**: Rules to move between states.
  - **Path Cost**: Total cost from start to goal.

---

### 2. Brute Force Search

- **Definition**: Uninformed search that blindly explores all possible paths.
- **Types**:
  - **Depth-First Search (DFS)**
  - **Breadth-First Search (BFS)**

---

### 3. Depth-First Search (DFS)

- **Strategy**: Explores as far as possible along each branch before backtracking.
- **Data Structure**: Stack (can use recursion).
- **Time Complexity**: O(b^m)  
  *(b = branching factor, m = max depth)*
- **Space Complexity**: O(m)
- **Advantage**: Low memory usage.
- **Disadvantage**: May get stuck in infinite loops if not careful.

---

### 4. Breadth-First Search (BFS)

- **Strategy**: Explores all nodes at the present depth before going deeper.
- **Data Structure**: Queue
- **Time Complexity**: O(b^d)  
  *(d = depth of goal node)*
- **Space Complexity**: O(b^d)
- **Advantage**: Guaranteed to find shortest path.
- **Disadvantage**: High memory usage.

---

### 5. Heuristic Search

- **Heuristic**: An estimate or rule of thumb that helps in decision making.
- **Used to**: Prioritize paths that seem more promising.
- **Heuristic Function (h(n))**: Estimates cost from node `n` to goal.

---

### 6. Hill Climbing

- **Strategy**: Move to neighbor with highest value (greedy).
- **Types**:
  - Simple Hill Climbing
  - Steepest-Ascent Hill Climbing
  - Stochastic Hill Climbing
- **Problem**: Gets stuck in local maxima, plateaus, or ridges.

---

### 7. Best First Search

- **Strategy**: Selects the most promising node based on heuristic value.
- **Data Structure**: Priority Queue
- **Evaluation Function**: `f(n) = h(n)`
- **Advantage**: Faster than BFS/DFS for large search spaces.

---

### 8. A* Algorithm

- **Evaluation Function**:  
  `f(n) = g(n) + h(n)`  
  - `g(n)` = cost from start to node `n`  
  - `h(n)` = estimated cost from `n` to goal  
- **Optimal and Complete**, if `h(n)` is **admissible** (never overestimates).
- **Time Complexity**: Exponential in worst case.
- **Widely used in**: Maps, games, robotics.

---

### 9. Beam Search

- **Modification of Best First Search**.
- Explores only **k-best nodes** at each level (beam width = k).
- **Advantage**: Less memory.
- **Disadvantage**: May miss optimal solution.

---

### 10. AO* Algorithm

- Used for solving problems that can be broken into **AND-OR graphs**.
- **AO* = A-star for AND-OR graphs**.
- Suitable for **problem reduction** and **planning** tasks.
- Selects nodes based on minimum cost path through an AND-OR tree.

---

### 11. Constraint Satisfaction Problems (CSPs)

- **Definition**: Problems defined by variables, domains, and constraints.
- **Examples**: Sudoku, Map Coloring, N-Queens.
- **Techniques**:
  - Backtracking
  - Forward Checking
  - Constraint Propagation (e.g., AC-3 algorithm)
- **Goal**: Assign values to variables such that all constraints are satisfied.

---

### Summary Table

| **Technique**      | **Type**         | **Uses Heuristic?** | **Key Features**                          |
| ------------------ | ---------------- | ------------------- | ----------------------------------------- |
| BFS                | Uninformed       | No                  | Complete, finds shortest path             |
| DFS                | Uninformed       | No                  | Low memory, may not find best solution    |
| Hill Climbing      | Heuristic        | Yes                 | Greedy, can get stuck                     |
| Best First Search  | Heuristic        | Yes                 | Uses `f(n) = h(n)`                        |
| A* Search          | Heuristic        | Yes                 | Optimal, uses `f(n) = g(n) + h(n)`        |
| Beam Search        | Heuristic        | Yes                 | Memory-efficient, approximate             |
| AO* Search         | Heuristic        | Yes                 | AND-OR graphs, planning                   |
| CSP (e.g., Sudoku) | Constraint-Based | No (usually)        | Variables + Constraints, solved via logic |

---
