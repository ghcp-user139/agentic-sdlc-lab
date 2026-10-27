---
applyTo: "tests/**"
description: "Use when creating or changing tests. Covers unit and integration test conventions, assertions, and test commands."
---

# Test Instructions

- Write a focused failing test before implementing a behavior change.
- Keep unit tests in `tests/unit/` at the service level: call services directly and use mocked repositories; do not require a database or HTTP client.
- Keep integration tests in `tests/integration/` at the API boundary: use the existing `TestClient` and database fixtures.
- Test one behavior per test and use the `test_<function>_<situation>` naming pattern.
- Assert observable results and relevant side effects, including failure behavior. Never weaken or remove an existing assertion to make a test pass.
- Reuse existing fixtures and helpers, and follow the nearby pytest style.
- Run unit tests with `make test-unit`; set `AUTH_JWT_SECRET_KEY` before running tests.
