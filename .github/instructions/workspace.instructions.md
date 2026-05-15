---
description: Workspace-level instructions for the Soc Ops repository.
---

# Soc Ops Workspace Instructions

## Mandatory development checklist

- `cd socops && ./mvnw test`
- `cd socops && ./mvnw clean package`
- Use linting or code formatting checks before submitting changes.

This repo is a Spring Boot + Thymeleaf social bingo game with a small frontend and workshop guide.

## Key conventions

- Use Maven wrapper in `socops/` for build, run, and test.
- Keep controllers thin; place game assembly and rules in `com.socops.service`.
- Render pages and endpoints from `com.socops.web`.
- Keep frontend styling in `socops/src/main/resources/static/css/app.css` and avoid heavy CSS frameworks.
- Add tests under `socops/src/test/java/com/socops/` using Spring Boot / JUnit patterns.

## Practical guidance

- Preserve model concepts like `BingoCell`, `WinningStreak`, and `PlayPhase`.
- Prefer semantic Thymeleaf HTML and concise utility classes.
- Avoid new dependencies unless clearly justified.
- Leave `workshop/` docs unchanged unless the task explicitly requires updates.
