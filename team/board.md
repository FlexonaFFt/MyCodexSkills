# Team Board

## Objective

- Goal: Refactor this repository into a simple backup store for personal Codex skills.
- Constraints: Keep the structure minimal; keep `team/` communication-only; change real repository files outside `team/`.
- Acceptance Criteria: Existing skill lives under `skills/`; additional personal skills from `~/.codex/skills` are copied into `skills/`; README describes the simple skills repository and install command; QA verdict and final summary are recorded.

## Tasks

- T1: Inspect current repository layout | Owner: TeamLead | Depends on: none | Status: done | DoD: Existing files and current structure are understood.
- T2: Move existing skill into `skills/autonomous-dev-team` | Owner: 01developer | Depends on: T1 | Status: done | DoD: Skill files are no longer at repository root and live under `skills/`.
- T3: Update README for the simplified repository structure | Owner: 02developer | Depends on: T2 | Status: done | DoD: README explains the personal skills store and install command.
- T4: Validate final layout | Owner: qatester | Depends on: T2,T3 | Status: done | DoD: Required files exist and old single-skill layout is gone.
- T5: Copy remaining personal skills from `~/.codex/skills` | Owner: 03developer | Depends on: T4 | Status: done | DoD: `karp`, `karpwrite`, and `ml-study-mode` exist under `skills/`.
- T6: Update README skill inventory | Owner: 02developer | Depends on: T5 | Status: done | DoD: README lists all copied personal skills.
- T7: Validate backup store contents | Owner: qatester | Depends on: T5,T6 | Status: done | DoD: All expected `SKILL.md` files are present.

## Notes

- `team/` remains communication-only.
- Real repository changes were made in `README.md` and `skills/`.
- The previous generated `dist/` artifact was removed to keep the repository simple.
- Copied personal skills only: `autonomous-dev-team`, `karp`, `karpwrite`, `ml-study-mode`.
