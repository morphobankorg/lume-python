# Changelog v1.0.0

## Breaking Changes

*   **Project Rename to Lume**
    The project has been renamed from `python-logging` to `Lume`.
    *   **Migration:** Update all import paths from `python-logging` to `lume`. Remove all references to legacy logging services.
    *   **Commits:** [8](https://github.com/aurumorinc/python-logging/commit/8), [9](https://github.com/aurumorinc/python-logging/commit/9), [20](https://github.com/aurumorinc/python-logging/commit/20)

*   **Python 3.11 Requirement**
    The project now requires Python 3.11 or higher.
    *   **Migration:** Ensure your runtime environment is upgraded to Python 3.11+. Update CI/CD pipelines and Dockerfiles to reflect this requirement.
    *   **Commits:** [87](https://github.com/aurumorinc/python-logging/commit/87), [88](https://github.com/aurumorinc/python-logging/commit/88), [91](https://github.com/aurumorinc/python-logging/commit/91)

*   **Logging Configuration Refactor**
    Replaced environment-based logging configuration with a new `stdout_format` Enum and refactored format functions.
    *   **Migration:** Replace environment-based configuration with the `stdout_format` Enum. Update existing logging format calls to use the new modular functions.
    *   **Commits:** [101](https://github.com/aurumorinc/python-logging/commit/101), [99](https://github.com/aurumorinc/python-logging/commit/99), [100](https://github.com/aurumorinc/python-logging/commit/100)

*   **Windmill Traceparent Rename**
    Renamed `get_windmill_context` to `get_windmill_traceparent` and updated the return type.
    *   **Migration:** Update all calls from `get_windmill_context` to `get_windmill_traceparent` and adjust handling logic for the new return type.
    *   **Commits:** [81](https://github.com/aurumorinc/python-logging/commit/81)

*   **Architecture & Coding Standards**
    Introduced global architectural rules, Domain-Driven Design (DDD) principles, and updated Python coding standards.
    *   **Migration:** Refactor existing codebases to align with the new DDD and global architectural rules.
    *   **Commits:** [34](https://github.com/aurumorinc/python-logging/commit/34), [120](https://github.com/aurumorinc/python-logging/commit/120), [121](https://github.com/aurumorinc/python-logging/commit/121)

*   **Versioning Scheme Reset**
    Reset versioning from date-based to semantic versioning (MAJOR.MINOR.PATCH).
    *   **Migration:** No code migration required; update internal documentation and release tracking to reflect the new semantic versioning scheme.
    *   **Commits:** [4](https://github.com/aurumorinc/python-logging/commit/4)

## Features

*   **Agent Skills Modules**
    Added documentation and skill modules for PostHog, Sentry, Windmill, and Langfuse.
    *   **Commits:** [26](https://github.com/aurumorinc/python-logging/commit/26), [29](https://github.com/aurumorinc/python-logging/commit/29), [30](https://github.com/aurumorinc/python-logging/commit/30)

*   **Core Project Initialization**
    Initialized project structure, including Pydantic settings, OpenTelemetry (OTel) integration, and core logging capabilities.
    *   **Commits:** [103](https://github.com/aurumorinc/python-logging/commit/103), [104](https://github.com/aurumorinc/python-logging/commit/104), [105](https://github.com/aurumorinc/python-logging/commit/105)

## Improvements

*   **Dependency Management**
    Upgraded project dependencies, added `colorama`, and removed redundant packages.
    *   **Commits:** [37](https://github.com/aurumorinc/python-logging/commit/37), [86](https://github.com/aurumorinc/python-logging/commit/86)

*   **Telemetry Refinements**
    Added processors to strip OTel IDs from logs and centralized OTel logic within the service module.
    *   **Commits:** [40](https://github.com/aurumorinc/python-logging/commit/40), [43](https://github.com/aurumorinc/python-logging/commit/43), [50](https://github.com/aurumorinc/python-logging/commit/50)

## Infrastructure

*   **CI/CD Pipeline**
    Implemented a centralized automated release workflow and updated job conditions.
    *   **Commits:** [54](https://github.com/aurumorinc/python-logging/commit/54), [71](https://github.com/aurumorinc/python-logging/commit/71), [72](https://github.com/aurumorinc/python-logging/commit/72)
