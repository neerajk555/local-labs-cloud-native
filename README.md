# Docker & Kubernetes: A Beginner-Friendly Course

Runs entirely on your own machine - no AWS account, no cost. This replaces the earlier, more terse version of
this track with a much more thorough, beginner-first course: every lab now includes a concept recap, guided
steps, self-try exercises, a comprehension quiz, and a common-mistakes section.

**Assumes no prior Docker or Kubernetes knowledge.** If you already know Docker well, you can likely start at
Module 3.

## How each lab is structured

- **Concept Recap** - the idea explained in plain language, before any commands
- **Steps** - guided, one small action at a time
- **Try It Yourself** - 1-2 exercises you do without step-by-step instructions (hints available if you get stuck)
- **Check Your Understanding** - a short quiz with answers, to confirm the concept actually landed
- **Common Mistakes** - the specific errors beginners hit on this exact topic

## Using VS Code

If you have VS Code installed, see **`USING-VSCODE.md`** for setup and recommended extensions. Any lab step
that creates a file via a terminal heredoc (`cat > file <<EOF ... EOF`) automatically includes a "Using VS Code
instead" box right underneath it, showing exactly what file to create and what to paste in — no need to
manually translate every heredoc yourself.

## Prerequisites (all modules)

- Docker Desktop (or Docker Engine on Linux)
- `kind` (from Module 4 onward)
- `kubectl` (from Module 4 onward)
- `helm` (Module 6 only)
- `openssl` (Module 7's TLS lab only)
- VS Code (optional but recommended - see `USING-VSCODE.md`)

## Modules

| Module | Topic | Labs |
|---|---|---|
| 0 | Containers 101 (concepts, minimal CLI) | 4 |
| 1 | Docker Basics | 11 (incl. mini-project) |
| 2 | Docker Compose | 10 (incl. mini-project) |
| 3 | Kubernetes Concepts (no CLI) | 4 |
| 4 | Kubernetes Basics with kind | 12 (incl. mini-project) |
| 5 | Workloads & Storage | 6 |
| 6 | Helm Basics | 6 |
| 7 | Ingress & Networking | 6 |
| 8 | Capstone Project | 1 (multi-part) |

**Total: 60 labs/exercises across 9 modules**, versus 25 in the previous version.

## Suggested pace

This is intentionally NOT a "do it all in a weekend" course. A reasonable pace for someone new to this material:

- Modules 0-2 (Docker): 1-2 weeks, a few labs per session
- Module 3 (K8s concepts): a single sitting - it's short and conceptual, but important not to skip
- Modules 4-5 (K8s core): 2-3 weeks, this is the bulk of the material
- Modules 6-7 (Helm, Ingress): 1 week
- Module 8 (Capstone): as long as it takes - this is meant to be genuinely challenging

## If you get stuck

Every lab's Common Mistakes section covers the most frequent beginner errors for that specific topic - check
there before searching elsewhere. The Check Your Understanding quizzes are also a good way to identify which
concept (not just which command) you're missing.
