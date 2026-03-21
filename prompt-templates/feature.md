Goal:
Implement a new feature in an existing Java 21 backend service.

Context:
- Tech stack: Java 21, Spring Boot
- The code should fit into an existing production codebase
- Prefer maintainable, readable, pragmatic design
- Follow clean code and SOLID principles, but do not overengineer
- Assume this is enterprise backend code, not coding challenge code

Coding style:
- Prefer readability over cleverness
- Keep methods and classes focused
- Prefer clear naming
- Use Lombok val for local variables where readability is not harmed
- Avoid unnecessary abstractions, generic layers, or patterns
- Reuse existing conventions if they are visible in the provided code
- Preserve backward compatibility unless explicitly told otherwise
- Do not introduce unnecessary dependencies
- Prefer explicit and understandable control flow
- If tradeoffs exist, choose the simpler production-friendly solution

Task:
[describe the feature clearly]

Relevant context:
[paste code, interface, DTOs, current flow, or service structure]

Constraints:
- Do not change public APIs unless necessary
- Do not break existing behavior unless explicitly requested
- Consider edge cases, validation, and failure handling
- Consider performance if relevant
- Consider idempotency / retries if relevant
- Consider database or messaging implications if relevant

Expected output:
1. Short implementation approach
2. Key design decisions
3. Proposed code changes
4. Example implementation
5. Edge cases and risks
6. Optional improvements if the current design has obvious issues

Important:
- If the requested implementation has architectural risks, say so first
- If the design is too vague, make reasonable assumptions and state them
- Do not return a giant wall of code without explanation