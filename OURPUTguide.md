# Developer Log (DEVLOG.md)
## Maze Escape (Spring 2026)

---
## Allowed Entry Types
Each entry may be one of the following:
1) **Bug Fix Entry**
- The issue encountered.
- Error messages or symptoms.
- Attempts made.
- Final resolution.
2) **Edge Case / Testing Entry**
- A failure discovered through testing.
- The specific input/state that caused it.
- The change you made to handle it correctly.
3) **Engineering Decision Entry (up to 2 allowed)**
- A design decision you made.
- An alternative approach you considered.
- Why you chose one approach over another (tradeoffs).
---
### Entry 1
**Date:** YYYY-MM-DD
**Entry Type:** Bug Fix / Edge Case / Engineering Decision
**Task worked on:**
**Issue or decision:**
**Error message / symptom (if applicable):**
**What I tried:**
**Fix / resolution (or final decision):**
**Commit(s):**
---
### Entry 2
**Date:** YYYY-MM-DD
**Entry Type:** Bug Fix / Edge Case / Engineering Decision
**Task worked on:**
**Issue or decision:**
**Error message / symptom (if applicable):**
**What I tried:**
**Fix / resolution (or final decision):**
**Commit(s):**
---
### Entry 3
**Date:** 2026-04-26 \
**Entry Type:** Edge Case \
**Task worked on:** Checking if a space is valid. \
**Issue or decision:** Choosing how to validate a space. \
**Error message / symptom (if applicable):** Random exit code because out of bounds accessing. \
**What I tried:** I landed on the solution with an error I solved later. \
**Fix / resolution (or final decision):** I added an if statement checking if the rows or cols are out of the array's 
bounds and a statement checking if we are on a wall
**Commit(s):**
Boudries Check
---
### Entry 4
**Date:**  2026-04-27 \
**Entry Type:** Edge Case \
**Task worked on:** Checking if a space is within a boundry. \
**Issue or decision:** It let in boundaries that were of the size of the array
**Error message / symptom (if applicable):** Random exit code. \
**What I tried:** The solution is all I tried. \
**Fix / resolution (or final decision):** I change the condition for being outside the array's bounds to >= from >. \
**Commit(s):**
Fixed Boundaries Check 1 
---
### Entry 5
**Date:** 2026-04-28
**Entry Type:** Bug Fix 
**Task worked on:** Showing the found path traceback \
**Issue or decision:** I was adding to the parent's array in the wrong space. \
**Error message / symptom (if applicable):** It would time out and give an error code. \
**What I tried:** My solution is what I tried. \
**Fix / resolution (or final decision):** I ended up realizing how the parent array worked and realized I should only 
add to it once I know it's correct so I moved the parent setting to the part when the maze has found a path or the 
"backtracking" in recursion terms. \
**Commit(s):**
Parent Array's Fix
---
### Entry 6
**Date:** 2026-04-29
**Entry Type:** Engineering Decision \
**Task worked on:** Refactoring \
**Issue or decision:** Creating a method to check if a space isValid \
**Error message / symptom (if applicable):** N/A
**What I tried:** I only tried one thing which was what ended up working \
**Fix / resolution (or final decision):** In class Manju showed us an example of how we shuld handle a dfs problem and
unlike my current solution she used a separate method to check if the recursion was valid so I made my own moving the
checks for invalidity to a new method. \
**Commit(s):** 
IsValidSpace()
