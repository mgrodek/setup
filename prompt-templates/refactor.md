Goal:
Refactor existing Java 21 code to improve readability, maintainability, and structure without changing behavior.

Context:
- Tech stack: Java 21, Spring Boot
- This is production code in an existing backend service
- Refactoring should be pragmatic and safe
- Prefer simpler structure, lower cognitive complexity, and better naming
- Follow clean code and SOLID principles, but avoid overengineering

Coding style:
- Prefer readability over cleverness
- Use Lombok val for local variables where readability is not harmed
- Keep methods focused and reasonably short
- Avoid introducing unnecessary abstractions
- Preserve existing public contracts unless explicitly allowed to change them
- Prefer explicit code over magic
- Do not add patterns just for the sake of patterns

Input code:
[paste code]

Refactoring goals:
[describe what bothers you: long method, duplicated logic, mixed responsibilities, poor naming, etc.]

Constraints:
- Preserve behavior
- Preserve backward compatibility unless explicitly allowed otherwise
- Avoid changing more than necessary
- Highlight any risky refactoring areas
- If tests are missing, mention what should be covered before deeper refactor

Expected output:
1. Main problems in current code
2. Refactoring strategy
3. Refactored code
4. Why this version is better
5. Risks and things to verify
6. Suggested tests if relevant

Important:
- If the code is acceptable and does not need heavy refactoring, say so
- Prefer incremental refactoring over large rewrites
- If there is a simpler solution than a “beautiful” one, prefer the simpler one