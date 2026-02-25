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
| Dev run | `mvn spring-boot:run` |
| Clean | `mvn clean` |

### API endpoints

| Method | Path | Response |
|--------|------|----------|
| GET | `/hello` | `Hello Maven!` (text/plain) |

### Notes

- Spring Boot 3.2.5 on Java 17+ (JDK 21 pre-installed).
- `mvn spring-boot:run` 启动后默认监听 `http://localhost:8080`。
- JUnit 5 via `spring-boot-starter-test`，含 MockMvc 集成测试。
- No external services, databases, or Docker containers are required.
- No lint tooling is configured; `mvn compile` serves as the static check (compiler warnings).
