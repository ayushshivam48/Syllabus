# Module III: Coding

## 1. Programming Practices
Good programming practices ensure code is readable, maintainable, and error-free.

- **Code Clarity**: Use descriptive names for variables, functions, and classes. Proper indentation and spacing improve readability.
- **Reusability**: Write functions or modules that can be reused across different parts of the program.
- **Modularization**: Divide a program into smaller, independent modules to improve clarity and maintainability.
- **Error Handling**: Use try-catch blocks, validations, and exception handling to make code robust.
- **Version Control**: Use tools like Git to track changes and collaborate with others efficiently.

## 2. Top-Down Approach
A design approach where the system is broken down from the top level into smaller components.

- Focuses on breaking a big problem into smaller sub-problems.
- Helps in understanding the overall structure before delving into details.

## 3. Bottom-Up Approach
A design strategy where development starts with the most basic components, which are then integrated into a complete system.

- Encourages development of reusable modules.
- Useful when components already exist or can be reused.

## 4. Structured Programming
A programming paradigm aimed at improving clarity by using control structures like sequence, selection (if/else), and iteration (loops).

- Avoids GOTO statements.
- Encourages logical flow and easier debugging.

## 5. Information Hiding
A principle where internal details of modules are hidden, exposing only necessary interfaces.

- Achieved using encapsulation.
- Enhances security and modularity.

## 6. Paired Programming
An agile software development technique in which two programmers work together at one workstation.

- Driver writes the code.
- Observer reviews each line as it is typed in.
- Improves code quality and facilitates knowledge sharing.


# Module IV: Software Design

## 1. Software Design Process
A process to translate software requirements into a blueprint for building the software.

### Steps:
- **Requirement Analysis**: The process of identifying, documenting, validating, and managing the needs and expectations of stakeholders for a new or modified product or system.
- **Architectural Design**: It defines the high-level structure, components, and interactions of a software system, acting as a blueprint for its development and ensuring it meets functional and non-functional requirements.
- **Detailed Design**: It translates high-level system architecture into concrete, implementable components, specifying data structures, algorithms, and module interactions, forming a detailed blueprint for software construction.

## 2. Design Objectives
- **Correctness**: Design should fulfill all requirements.
- **Efficiency**: Optimize performance and resource use.
- **Flexibility**: Easy to adapt to changes.
- **Maintainability**: Easy to fix bugs and update.
- **Reusability**: Design should support reuse of components.

## 3. Structured Design Methodologies
A systematic approach that emphasizes clarity, maintainability, and ease of understanding by breaking down complex systems into smaller, manageable modules, often using techniques like top-down design and modularity.

- Use DFDs (Data Flow Diagrams), ERDs (Entity-Relationship Diagrams), and flowcharts.

## 4. Modules Coupling
Degree of interdependence between software modules.

- Lower coupling means better maintainability and independence.

## 5. Types of Coupling
- **Content Coupling**: One module modifies the content of another.
- **Common Coupling**: Modules share global data.
- **Control Coupling**: One module controls another by passing control info.
- **Stamp Coupling**: Modules share composite data structures.
- **Data Coupling**: Modules share data through parameters (most desirable).

## 6. Module Cohesion
Measure of how strongly elements of a module are related.

- Higher cohesion indicates better module design.

## 7. Types of Cohesion
- **Coincidental**: Elements are unrelated.
- **Logical**: Similar functions grouped together.
- **Temporal**: Elements are related by time of execution.
- **Procedural**: Elements execute in a specific sequence.
- **Communicational**: Operate on the same data.
- **Sequential**: Output of one part is input for another.
- **Functional**: Performs a single, well-defined task (most desirable).

## 8. Structured Chart
A visual representation of the logical structure of a system, often used in software engineering and organizational theory to show the relationships between modules or components.

- Helps visualize system architecture.

## 9. Qualities of Good Software Design
- **Modularity**: Divided into separate modules.
- **Scalability**: Can handle growth.
- **Maintainability**: Easy to update.
- **Performance**: Efficient operation.
- **Reusability**: Components can be reused.
- **User -friendliness**: Easy to use.
