# Contribution [#]: [Issue Title]

**Contribution Number:** [2]
**Student:** [Krishna Sai Sevilimedu Veeravalli]
**Issue:** [https://github.com/ProjectX-VJTI/Xplore-workshop/issues/28]
**Status:** [Phase I Complete]

---

## Why I Chose This Issue

[1-2 paragraphs explaining why this issue interests you, how it matches your skills/learning goals, what you hope to learn]

I chose this issue because it gives me a concrete chance to practice debugging and fixing real Python code, which is essential for my growth as a developer.
By fixing the bugs in `test_playground/intermediate/`, I help improve the learning experience for future students who rely on this repository.
Working through this issue strengthens my ability to spot logical errors, write defensive code, and produce clean, well‑documented solutions.
---

## Understanding the Issue

### Problem Description

[In your own words, what's broken or missing?]

### Expected Behavior

[What should happen?]

### Current Behavior

[What actually happens?]

### Affected Components

[Which parts of the codebase are involved?]

---

## Reproduction Process

### Environment Setup

- Clone the Fork
    ```
        https://github.com/krishnasai453/Xplore-workshop.git
        cd CoC-git-python-workshop
    ```
- Creating Solutions Folder
    krishnasai453_solutions/

- Copied the playground
    ```
        SOLUTIONS
        └── <githubid>_solutions/
            └── test_playground/
    ```

- Set Up Virtual Environment
    ```
        python3.12 -m venv venv
        source venv/bin/activate
    ```
- Install dependencies:
    ```
        pip install -r requirements.txt
    ≈

### Errors Faced During Environmenr Setup:
    Faced Following error while installing dependencies
    ```
        Building wheel for pygame (pyproject.toml) ... error
        error: subprocess-exited-with-error

        × Building wheel for pygame (pyproject.toml) did not run successfully.
        │ exit code: 1
        ╰─> [14 lines of output]
            src_c/_sdl2/sdl2.c:1237:10: fatal error: 'SDL.h' file not found
            1237 | #include "SDL.h"
                    |          ^~~~~~~
            1 error generated.
            Skipping Cython compilation

            ---
            For help with compilation see:
                https://www.pygame.org/wiki/MacCompile
            To contribute to pygame development see:
                https://www.pygame.org/contribute.html
            ---

            error: command '/usr/bin/clang' failed with exit code 1
            [end of output]

        note: This error originates from a subprocess, and is likely not a problem with pip.
        ERROR: Failed building wheel for pygame
        Failed to build pygame

        [notice] A new release of pip is available: 26.1 -> 26.1.2
        [notice] To update, run: pip install --upgrade pip
        error: failed-wheel-build-for-install

        × Failed to build installable wheels for some pyproject.toml based projects
        ╰─> pygame
    ```
    Fix::
        Updated package version and fixed the error

[Notes on setting up your local development environment - challenges you faced, how you solved them]



### Reproduction Evidence

- **Commit showing reproduction:** [Link to commit in your fork]
- **Screenshots/logs:** [If applicable]
- **My findings:** [What you discovered during reproduction]

---

## Solution Approach(UMPIRE)


U — Understand
Read the issue description and confirm the goal: fix the broken behavior in the files under intermediate.
Review the existing helper functions and the hints already embedded in:
dict_ops.py
json_handler.py
some_functions.py
sql_handler.py
txt_handler.py

M — Minimize
Keep the scope limited to the bug fixes in those intermediate exercises.
Avoid refactors or redesigns unless needed for correctness.
Fix only the broken logic described by the comments and expected behavior.

P — Prepare
Create a feature branch for the work.
Reproduce the current behavior by running each script or exercising the functions manually.
Note the expected output for each function before changing code.

I — Implement
Fix the logic in each target file:
In dict_ops.py, preserve falsy keys, apply latest values in merge logic, and count keys using the intended prefix behavior.
In json_handler.py, raise a proper error for missing files, handle empty key paths safely, and return success values correctly.
In some_functions.py, correct Fibonacci indexing, factorial logic, prime-check behavior, GCD termination, and sum-of-squares math.
In sql_handler.py, preserve decimal values, sort ascending by id, update only the targeted row, and delete the correct item.
In txt_handler.py, stop altering content unexpectedly, use append mode correctly, support zero-based line updates, and preserve file formatting.

R — Review
Run the scripts again and verify they now align with the intended behavior.
Check that no unrelated files were changed.
Review the diff for clarity and minimality.

E — Evaluate
Confirm the bug is resolved and the output now matches the expectations described in the issue.
Prepare a short PR description with:
what was fixed,
files changed,
how it was validated.

### Analysis

[Your analysis of the root cause - what's causing the issue?]

### Proposed Solution

[High-level description of your fix approach]

### Implementation Plan

Using UMPIRE framework (adapted):

**Understand:** [Restate the problem]

**Match:** [What similar patterns/solutions exist in the codebase?]

**Plan:** [Step-by-step implementation plan]
1. [Modify file X to do Y]
2. [Add function Z]
3. [Update tests]

**Implement:** [Link to your branch/commits as you work]

**Review:** [Self-review checklist - does it follow the project's contribution guidelines?]

**Evaluate:** [How will you verify it works?]

---

## Testing Strategy

### Unit Tests

- [ ] Test case 1: [Description]
- [ ] Test case 2: [Description]
- [ ] Test case 3: [Description]

### Integration Tests

- [ ] Integration scenario 1
- [ ] Integration scenario 2

### Manual Testing

[What you tested manually and results]

---

## Implementation Notes

### Week [X] Progress

[What you built this week, challenges faced, decisions made]

### Week [Y] Progress

[Continue documenting as you work]

### Code Changes

- **Files modified:** [List]
- **Key commits:** [Links to important commits]
- **Approach decisions:** [Why you chose certain approaches]

---

## Pull Request

**PR Link:** [GitHub PR URL when submitted]

**PR Description:** [Draft or final PR description - much of the content above can be adapted]

**Maintainer Feedback:**
- [Date]: [Summary of feedback received]
- [Date]: [How you addressed it]

**Status:** [Awaiting review / Iterating / Approved / Merged]

---

## Learnings & Reflections

### Technical Skills Gained

[What you learned technically]

### Challenges Overcome

[What was hard and how you solved it]

### What I'd Do Differently Next Time

[Reflection on your process]

---

## Resources Used

- [Link to helpful documentation]
- [Tutorial or Stack Overflow post that helped]
- [GitHub issues or discussions that helped]
