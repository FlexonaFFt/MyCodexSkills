---
name: karp
description: Coding discipline for implementation, bug fixes, and refactors where Codex should think before coding, state assumptions, avoid overengineering, make surgical changes, and verify against tests or explicit success criteria. Use when the user asks Codex to write, edit, fix, or refactor code and wants minimal, goal-driven engineering behavior.
---

# Karp

## Overview

Use this skill to keep coding work narrow, explicit, and verifiable. Prefer the smallest correct change that satisfies the request and matches the existing codebase.

## Workflow

1. State assumptions before coding.
2. List plausible interpretations when the request is ambiguous.
3. Ask a clarifying question if choosing an interpretation would be risky or likely to waste work.
4. Propose the simpler approach when one exists, with a short reason.
5. Define success criteria or tests before changing code.
6. Make only the edits required for the task.
7. Verify the result with the narrowest meaningful test, command, or inspection.

## Coding Rules

- Write the minimum code that solves the stated problem.
- Avoid new features, abstractions, configuration, dependencies, and patterns unless the task requires them.
- Match the existing style, naming, layout, and test conventions.
- Change only files and lines needed for the request.
- Do not refactor unrelated code, comments, or formatting.
- Remove only unused elements that became dead because of your changes.
- If the implementation grows longer than needed, simplify it before finishing.

## Verification Rules

- For bug fixes, first describe or add a failing test or concrete reproduction, then fix the bug.
- For refactors, preserve behavior according to existing tests or a stated specification.
- For multi-step tasks, outline a short plan with verification for each step before execution.
- Prefer focused tests over broad test suites unless the change touches shared behavior.
- If no automated test is practical, state the manual verification or code inspection used.

## Communication Rules

- Be explicit about uncertainty.
- Do not silently choose between materially different interpretations.
- Keep plans and explanations short unless the task needs detail.
- Stop and ask when the task is unclear enough that implementation would be guesswork.
