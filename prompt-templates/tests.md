Goal:
Generate meaningful tests for Java 21 backend code.

Context:
- Testing stack: JUnit 5, AssertJ
- Mockito can be used if needed
- Focus on behavior, not implementation details
- Tests should be readable, maintainable, and useful in production codebase
- Prefer high signal tests over noisy tests

Coding style:
- Use JUnit 5
- Use AssertJ for assertions
- Prefer descriptive test names
- Cover happy path, edge cases, and negative scenarios
- Keep tests easy to read
- Mock only where it makes sense
- Do not create brittle tests tightly coupled to implementation details
- Prefer testing business behavior over internal method structure

Input:
[paste class / method / service / code fragment]

Testing focus:
[describe what you care about: validation, mapping, retries, exception handling, business rules, etc.]

Constraints:
- Preserve current public behavior
- If mocking is needed, keep it minimal and reasonable
- If the code is hard to test, explain why
- If the class design hurts testability, mention it

Expected output:
1. List of important test cases
2. Example test class
3. Edge cases that should not be missed
4. Potential testability issues in the production code
5. Suggestions for improving testability if relevant

Important:
- Use AssertJ assertions
- Prefer behavior-oriented tests
- Include negative cases and boundary conditions
- If integration test would be better than a unit test for some scenario, say so