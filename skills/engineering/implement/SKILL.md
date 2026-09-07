---
name: implement
description: "Implement a piece of work based on a spec or set of tickets."
disable-model-invocation: true
---

Implement the work described by the user in the spec or tickets.

Before writing any new code, climb the ponytail ladder and stop at the first rung that holds:
does this need to exist at all (YAGNI) → is it already in this codebase → does the stdlib do it →
does a native platform feature cover it → does an already-installed dependency solve it → can it
be one line → only then, the minimum code that works. No unrequested abstractions, no scaffolding
for later.

Use /tdd where possible, at pre-agreed seams.

Run typechecking regularly, single test files regularly, and the full test suite once at the end.

Once done, use /simplify to strip anything that crept past the ladder, then /code-review to review the work.

Commit your work to the current branch.
