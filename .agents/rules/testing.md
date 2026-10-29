# Testing rules

- Add or update automated tests for changed behavior when the application has a test harness.
- Choose an automated testing framework for each application, document its test command, and run the relevant test suite for every task that changes application behavior.
- Keep the `tests/` directory current with the application and its acceptance criteria.
- Run the narrowest relevant checks first, then broader checks when warranted.
- Do not claim verification that was not performed.
- Report commands run, outcomes, and any checks that could not run.
