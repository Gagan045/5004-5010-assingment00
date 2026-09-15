# LLM Code Evaluation Report — Assignment 0: Setup

> Copy this file to `LLM-Evaluation.md`, fill it in, and commit it. A0 is a **practice run** of the
> self-evaluation habit you'll use all term — the code is trivial, the workflow is the point.

## Student Information
- **Name**: Gagan
- **Date**: 2026-09-14
- **LLM Used**: Copilot / ChatGPT-style review

## Prompt Used
I used the assignment prompt to ask whether the Greeting class included my name, whether the tests would pass, and whether the build output showed a clean run.

## What the LLM said
The greeting string is exactly: "Hello, Java! — Gagan".

The JUnit test should pass because the message is non-blank and no longer contains the placeholder text. `STUDENT_NAME` stores the student name, and `message()` combines the fixed greeting prefix with that name. The tool output shows a clean run: `./gradlew run` printed the greeting, and the build/test/report tasks all ended with `BUILD SUCCESSFUL`.

## Your checklist
- **`./gradlew run` prints the greeting with my name?**: Yes
- **`./gradlew test` is green?**: Yes
- **Coverage + checkstyle reports generated?**: Yes
- **I can explain what `Greeting.message()` returns and why the test passes?**: Yes

## Reflection
This setup worked smoothly once the project was opened with the correct Java environment and the Gradle wrapper was used. The main lesson was that using `./gradlew` is important because it ensures the exact project-managed Gradle version and avoids environment mismatch issues.
