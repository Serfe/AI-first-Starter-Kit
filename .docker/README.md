# Docker environment

Use this directory for Docker files that make the project reproducible in containers.

Choose the Docker strategy that fits the project:

- **Test-only environment:** provide the dependencies and command required to run the automated test suite in a container.
- **Full application environment:** provide the application and its required services so the complete stack can run locally.

Document the selected approach, setup commands, and available Docker services in `app/README.md` once the application strategy is defined.
