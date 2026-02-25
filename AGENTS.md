# AGENTS.md

## Cursor Cloud specific instructions

This is a Java Maven project (`simple-maven-project`). The application entry point is `com.example.App` which prints "Hello Maven!".

### Prerequisites

- JDK 8+ (JDK 21 is pre-installed on the VM)
- Apache Maven 3.x (installed via `apt-get install maven`)

### Common commands

| Task | Command |
|------|---------|
| Build | `mvn compile` |
| Test | `mvn test` |
| Package | `mvn package` |
| Run | `java -cp target/simple-maven-project-1.0-SNAPSHOT.jar com.example.App` |
| Clean | `mvn clean` |

### Notes

- The project targets Java 1.8 source/target but compiles fine on JDK 21.
- JUnit 4.13.2 is the only dependency (test scope).
- No external services, databases, or Docker containers are required.
- No lint tooling is configured; `mvn compile` serves as the static check (compiler warnings).
