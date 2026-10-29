# R001: Add a visible application health endpoint

## Goal

Expose a `GET /health` endpoint that reports whether the example application is available.

## Acceptance criteria

- The endpoint returns HTTP 200.
- The response is JSON and includes `status: "ok"`.
- An automated test covers the successful response.
- Setup and test instructions are updated if an application is added.

## Out of scope

Authentication, external dependency checks, and production monitoring.
