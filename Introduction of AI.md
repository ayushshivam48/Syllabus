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

## Module III: Game Playing

---

### 1. AI and Game Playing

- **Definition**:  
  Game playing in AI refers to building agents that can play games intelligently by making optimal decisions based on the current game state.

- **Purpose**:
  - To simulate intelligent behavior.
  - To test decision-making algorithms.
  - To understand adversarial search.

- **Game Types**:
  - **Deterministic vs. Non-deterministic** (chance involved or not)
  - **Perfect Information vs. Imperfect Information**
  - **Zero-Sum Games**: One player's gain is another's loss (e.g., Chess, Tic-Tac-Toe).

---

### 2. Plausible Move Generator

- **Definition**:  
  A function that generates a subset of **possible legal moves** that appear to be **plausible or promising**.

- **Why used?**
  - To reduce the **search space**.
  - Improve **efficiency** of game-tree evaluation.
  - Useful in complex games (e.g., Chess) where exploring all moves is impractical.

---

### 3. Static Evaluation Function

- **Definition**:  
  A function that estimates the **goodness** of a position without doing any further search.

- **Used when**:
  - The game tree cannot be searched to terminal nodes due to complexity.

- **Example**:
  - In Chess, evaluation may consider:
    - Material balance
    - Piece positioning
    - Control of the center
    - King safety

---

### 4. Game Playing Strategies

#### i. Minimax Algorithm:
- Used for **two-player** games.
- Assumes both players play optimally.
- Max player tries to maximize the score; Min player tries to minimize it.

#### ii. Alpha-Beta Pruning:
- Optimized version of Minimax.
- Prunes branches that won't influence the final decision.
- Improves efficiency by reducing the number of nodes evaluated.

#### iii. Cut-off Search:
- Limits the depth of search tree.
- Uses **static evaluation** at the cut-off depth.

#### iv. Expectiminimax:
- Used for games with **chance elements** (e.g., Backgammon).
- Combines Minimax with **probabilities** at chance nodes.

---

### 5. Problems in Game Playing

| **Problem**                 | **Explanation**                                                                   |
|-----------------------------|-----------------------------------------------------------------------------------|
| **Combinatorial Explosion** | Number of possible moves increases exponentially (e.g., Chess has 10^120 states). |
| **Real-time Constraints**   | AI must make decisions in limited time.                                           |
| **Imperfect Information**   | In games like Poker, not all information is visible.                              |
| **Resource Limitation**     | Memory and processing power limitations prevent full search.                      |
| **Evaluation Inaccuracy**   | Static evaluation functions may misjudge complex positions.                       |

---

### Summary Table

| **Concept**                | **Description**                                                               |
|----------------------------|-------------------------------------------------------------------------------|
| AI in Game Playing         | Making intelligent agents to play games optimally                             |
| Plausible Move Generator   | Selects promising moves to reduce computation                                 |
| Static Evaluation Function | Evaluates non-terminal game states                                            |
| Minimax                    | Decision-making strategy for two-player games                                 |
| Alpha-Beta Pruning         | Skips unnecessary branches in game tree                                       |
| Expectiminimax             | Handles chance in games                                                       |
| Common Problems            | Combinatorial explosion, limited time, imperfect info, evaluation limitations |

---

## Module IV: Logic and Knowledge Representation

---

### PART A: Knowledge Representation (KR)

> **Definition**: Knowledge Representation is a method used to structure and store knowledge in a format that an AI system can utilize to solve complex tasks like diagnosis, planning, or learning.

---

#### 1. Associative Networks (Semantic Networks)

- **Graph-based structure** of nodes (concepts) and links (relations)
- **Used for** representing knowledge in a network of related ideas

**Example**:

Dog → is-a → Animal
Dog → has → Tail


- **Types of Links**:
  - **Is-a** (inheritance)
  - **Has-a** (attribute/property)
  - **Part-of**

---

#### 2. Frame Structures

- A **data structure** for representing a stereotyped situation
- Each frame consists of **slots** (attributes) and **fillers** (values)

**Example**:

Frame: Car

Type: Vehicle

Wheels: 4

Engine: Yes


- Supports **inheritance**, **default values**, and **procedural attachment**

---

#### 3. Conceptual Dependencies (CD)

- Used for **natural language understanding**
- Represents meaning using **primitive actions** and fixed relations

**Key primitives**:
- **PTRANS** – physical transfer (e.g., go)
- **ATRANS** – abstract transfer (e.g., give)
- **MTRANS** – mental transfer (e.g., tell)
- **PROPEL** – apply force

**Example**:

"John gave a book to Mary" → ATRANS(John, Book, Mary)


---

#### 4. Scripts

- Structured knowledge for **event sequences**
- Represent **standard scenarios** (e.g., restaurant visit)

**Script: Restaurant**:

Entry → Ordering → Eating → Paying → Exit


- Helps AI understand **contextual expectations**

---

### PART B: Logic

> Logic is used to **reason** and **infer** new information from known facts.

---

#### 1. Propositional Logic

**Syntax**:
- Propositions (P, Q, R...)
- Connectives: AND (∧), OR (∨), NOT (¬), IMPLIES (→), IFF (↔)

**Semantics**:
- Each proposition is **true/false**
- Uses **truth tables** for evaluation

---

#### 2. First Order Predicate Logic (FOPL)

**Syntax**:
- Extends propositional logic with:
  - **Predicates**: P(x), Loves(John, Mary)
  - **Quantifiers**:
    - ∀ (For all)
    - ∃ (There exists)
  - Variables, Constants, Functions

**Semantics**:
- Based on **interpretations and domains**
- Assigns meaning to constants, predicates, functions

---

#### 3. Conversion to Clausal Form

> Required for resolution-based inference

**Steps**:
1. Eliminate bi-conditionals and implications
2. Move NOT inward (De Morgan's laws)
3. Standardize variables
4. Move quantifiers to front (Prenex form)
5. Skolemize (remove existential quantifiers)
6. Drop universal quantifiers
7. Convert to **CNF (Conjunctive Normal Form)**

---

#### 4. Inference Rules

**Common rules**:
- **Modus Ponens**: If P → Q and P, then Q
- **Modus Tollens**: If P → Q and ¬Q, then ¬P
- And-Elimination, Or-Introduction

---

#### 5. Unification

- Makes two logical expressions **identical** via substitution
- Used in **automated reasoning** and **Prolog**

**Example**:

Loves(x, y) and Loves(John, y) → x = John


---

#### 6. Resolution Principle

- Main inference rule in FOPL
- Based on **refutation** (proof by contradiction)
- Works on **clausal form (CNF)**

**Example**:
1. ¬P ∨ Q
2. P
→ Resolve: Q

---

### Summary Table

| Concept                 | Description                                      |
|-------------------------|--------------------------------------------------|
| Associative Network     | Graph of concepts with relationships            |
| Frame Structure         | Slots and values for stereotypes                |
| Conceptual Dependency   | Action primitives for language understanding    |
| Script                  | Standard event sequences                        |
| Propositional Logic     | Boolean statements and operators                |
| Predicate Logic (FOPL)  | Adds predicates, quantifiers                    |
| Clausal Form            | CNF format for resolution                       |
| Unification             | Matching expressions via substitution           |
| Resolution Principle    | Derives contradictions to prove conclusions     |
