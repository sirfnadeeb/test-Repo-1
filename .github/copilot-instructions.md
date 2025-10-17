# Copilot instructions for test-Repo-1

This repository is a very small test/demo Java project. The goal of these instructions is to help an AI coding agent be immediately productive when making small edits, adding examples, or improving the Java demo.

What this repo contains
- `README.md` — short repo description.
- `test file 1` — a Java program (`AddStrings.java`) that reads two strings and prints concatenations (plain concatenation and StringBuilder).

High-value work an agent can do
- Improve Java example code (`AddStrings.java`) for robustness, formatting, and Java conventions.
- Rename `test file 1` to a proper filename (`AddStrings.java`) under a `src/` folder and add a simple build/run workflow.
- Add a README snippet showing how to compile/run the Java program on Windows PowerShell.

Project-specific patterns & conventions
- This repo currently uses a single Java example in a plain text file named `test file 1`. Treat that file as source code. Prefer conventional Java file naming when editing (class name must match filename).
- Keep changes minimal and explain why — this is a learning/test repo; avoid introducing heavy tooling unless asked.

Build / run / debug notes
- No build system (Maven/Gradle) exists. For quick runs on Windows PowerShell use:
  - Compile: `javac AddStrings.java`
  - Run: `java AddStrings`
- If you move sources into `src/` create a minimal `compile` step in the README or add a `build.bat` / `build.ps1` script.

Integration & external deps
- None detected. Avoid adding external dependencies without user confirmation.

Helpful examples from this repo
- `test file 1` contains the working Java code. When refactoring, keep the same IO behavior (reads two lines from stdin, prints two concatenations).

Agent constraints and guardrails
- Do not replace the simple example with an unrelated project scaffold unless the user asks.
- Preserve the core behavior of the sample when refactoring (input prompts and both concat outputs).
- When renaming files, update README and any instructions accordingly.

If you need to make larger changes (add Maven, tests, CI), ask the user before proceeding.

---
If any part of this guidance is unclear or you'd like broader changes (tests, CI, packaging), tell me which direction and I will update the file.