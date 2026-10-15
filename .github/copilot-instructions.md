# Soc Ops Workspace Instructions

## Mandatory Development Checklist

- [ ] Lint or perform the closest available static validation for changed files.
- [ ] Run `mvnw.cmd clean package` from `socops/`.
- [ ] Run `mvnw.cmd test` from `socops/`.
- [ ] Review the diff and report any validation that could not run.

## Project and Commands

- Java 21 Spring Boot 3.x social bingo app in `socops/`, using Maven, Thymeleaf, and static assets.
- Run commands from `socops/` with `./mvnw` or Windows `mvnw.cmd`; start with `mvnw.cmd spring-boot:run`.
- Keep tests in `socops/src/test/java/` using JUnit 5. Never modify generated files under `socops/target/`.

## Conventions

- Preserve Java 21 and the current Spring Boot setup. Follow `com.socops` packages: `model`, `service`, `web`, and `data`.
- Keep business logic in services/models, use existing Spring MVC patterns, and preserve API response shapes.
- Prefer immutable data, descriptive names, and existing JDK/Spring libraries over new dependencies.

## Web UI and Editing

- Put templates in `socops/src/main/resources/templates/` and assets in `socops/src/main/resources/static/`.
- Follow `.github/instructions/css-utilities.instructions.md` and `.github/instructions/frontend-design.instructions.md` for UI work.
- Keep the game responsive and free of overlapping controls; prefer CSS-only motion.
- Make the smallest focused change, preserve unrelated work, avoid broad reformatting, and do not commit unless asked.
- For endpoint or domain changes, add or update focused tests.
- Review the diff for unnecessary files, generated output, stale documentation, and behavior changes.


