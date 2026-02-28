# AGENTS.md - Guidelines for AI Coding Agents

These guidelines are designed to ensure the consistent, maintainable, and high-quality development of AI coding agents within this repository. Adherence to these principles is mandatory for all development activities.

## 1. DRY (Don't Repeat Yourself)

*   **Single Responsibility Principle:** Each agent should have a single, well-defined purpose. Avoid creating overly complex agents with multiple functions or modules that perform similar tasks.
*   **Abstraction:** Utilize abstraction to decouple concerns.  Create interfaces and abstract classes to represent common functionalities and reduce code duplication.
*   **Standardized Components:**  Define and standardize reusable components whenever possible.  Document the purpose and usage of each component thoroughly.

## 2. KISS (Keep It Simple, Stupid)

*   **Minimalism:** Strive for the shortest possible solution that achieves the desired functionality. Avoid unnecessary complexity.
*   **Readability:** Prioritize clear, understandable code. Use meaningful variable names and comments where necessary but avoid excessive commenting.
*   **Focus on Core Logic:** Keep the agent's core logic focused on its primary task.  Don't introduce tangential features unless absolutely necessary.

## 3. SOLID Principles

*   **Single Responsibility:** Agents with a single responsibility principle are easier to test and maintain.
*   **Open/Closed Principle:**  The agent's design should be open for extension but closed for modification.  New functionality should be added via new agents, not by modifying existing ones.
*   **Liskov Substitution Principle:**  Objects of derived classes should be substitutable for objects of their base classes without altering the correctness of the program.  (This principle is less critical for pure AI agent logic, but emphasizes design choices.)
*   **Interface Segregation Principle:**  Clients should not be forced to provide the implementation details of an abstraction.

## 4. YAGNI (You Aren't Gonna Need It)

*   **Future-Proofing:** Only implement functionality that is currently required. Avoid designing features that might be needed in the future.
*   **Avoid Feature Creep:** Resist the urge to add new functionality without a clear justification.  Feature requests should be carefully evaluated and prioritized.

## 5. Code Quality & Structure

*   **Error Handling:** Implement robust error handling to prevent unexpected crashes or data loss.  Log errors effectively.
*   **Data Structures:** Choose appropriate data structures for each agent's purpose.  Consider efficiency and maintainability.
*   **Code Formatting:**  Adhere to consistent code formatting style (e.g., using a linter).
*   **Comments:** Provide clear and concise comments to explain complex logic or non-obvious code.  Comments should explain *why*, not just *what*.

## 6. Development Practices

*   **Unit Testing:** All agent code must be thoroughly tested with unit tests.  Aim for 80% test coverage.
*   **Integration Testing:**  Perform integration tests to ensure agents work correctly together.
*   **Code Reviews:** All code changes must undergo peer review before merging.
*   **Documentation:** Provide clear documentation for each agent, including its purpose, inputs, outputs, and potential side effects.
*   **Version Control:** Utilize a version control system (e.g., Git) for all agent code.

## 7.  Maximum Code Length: 180 Lines

*   All code must be within the specified line limit.

## 8.  Test Coverage: 80%

*   All tests must achieve 80% test coverage. Automated tests must be defined and executed on every code commit.

## 9.  File Structure (Example)

*   **agents.py:**  Core agent logic, data representation, and interaction methods.
*   **data_models.py:** Define data models and schemas for agents.
*   **components.py:**  Reusable agent components (e.g., message handlers, data processing routines).
*   **tests.py:**  Unit and integration tests for agents.
*   **utils.py:**  Utility functions and helper classes.

## 10.  Specific Considerations for AI Agents

*   **State Management:**  Clearly define and manage agent states.
*   **Learning:**  If the agent incorporates learning, document the learning process and ensure it’s well-controlled.
*   **Safety:**  Consider safety mechanisms to prevent unintended consequences during operation.

These guidelines are intended as a baseline.  Ongoing refinement and adjustment may be necessary as the project evolves. Any deviations from these guidelines will be subject to review.