---
name: clout-security-perf-audit
description: Audit implemented code for OWASP security vulnerabilities, database bottlenecks, concurrency issues, and generate load test scenarios.
---

# clout-security-perf-audit

Perform a rigorous security, performance, and reliability gate review across completed backend and frontend deliverables before release.

## When To Use

- Use this skill when reviewing completed implementation subtasks or pull requests prior to final human sign-off.

## Workflow

1. Inspect all modified backend and frontend files against the approved spec.md acceptance criteria and architecture contracts.
2. Audit for security vulnerabilities including injection, broken access control, missing input validation, sensitive data exposure, and insecure CORS or auth configurations.
3. Audit for performance bottlenecks including JPA N+1 queries, missing PostgreSQL indexes, blocking calls on virtual threads, and unnecessary Angular re-renders.
4. Produce a structured English Go or No-Go audit report listing severity-ranked findings with exact file references and concrete fixes, plus a Locust load test script for critical endpoints.