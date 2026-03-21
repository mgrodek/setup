Goal:
Review a code change in a Java 21 backend system that may involve batch processing, Kafka, data pipelines, or large payload handling.

Context:
- Tech stack: Java 21, Spring Boot
- Production system
- Code may run in distributed or retryable environment
- System may process large datasets or large payloads
- Review should focus on correctness, resilience, performance, and operational safety
- Prefer practical comments over cosmetic comments

Coding style expectations:
- Prefer readability over cleverness
- Use Lombok val for local variables where readability is not harmed
- Prefer clear naming and focused methods
- Avoid unnecessary abstractions
- Preserve backward compatibility unless explicitly allowed otherwise
- Prefer simple and maintainable solutions

Input:
[paste code diff, PR summary, changed files, or describe the branch changes]

System specific review focus:
- correctness under retries
- idempotency where relevant
- duplicate processing risks
- failure handling and partial failure behavior
- memory usage and large input safety
- unnecessary object copying
- blocking operations inside heavy processing paths
- ordering assumptions if messages or batches are involved
- database interaction efficiency
- transactional boundaries
- observability impact (logs, metrics, traceability)

Review questions:
1. Can this break under retry or duplicate execution?
2. Can this create memory or performance problems on larger inputs?
3. Does this introduce hidden coupling or unclear side effects?
4. Are failure scenarios handled explicitly enough?
5. Is the code easy enough to debug in production?
6. Are tests sufficient for risky paths?

Expected output:
1. Short summary of what the change does
2. Critical issues
3. Medium risk issues
4. Performance or scalability concerns
5. Retry / idempotency concerns
6. Test gaps
7. Suggested improvements
8. Positive notes

Important:
- Prioritize correctness and production risks over style nitpicks
- If there are no serious problems, say that clearly
- Distinguish between must fix and nice to improve
- If more context is needed, state assumptions explicitly