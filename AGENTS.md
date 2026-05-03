# Mathematics Study Repository

Learning maths again, but this time not for the grades.

## Syllabus

Master syllabus: [`real-analysis/syllabus.md`](real-analysis/syllabus.md) — 9 sprints of rigorous Real Analysis, 2 weeks each.

## Directory Structure

```
maths/
├── AGENTS.md                      # ← You are here (hub + tracking guide)
├── README.md                      # Original minimal readme
├── macros.tex                     # Shared LaTeX macros
├── flake.nix / flake.lock         # Nix dev environment
├── .github/ISSUE_TEMPLATE/        # GitHub issue templates
│   ├── notes.md                   # Week 1 self-study template
│   └── pset.md                    # Week 2 problem set template
└── real-analysis/
    ├── syllabus.md                # Master syllabus file
    ├── template.tex               # LaTeX template for notes/psets
    ├── notes/                     # Lecture notes per sprint
    ├── problem-sets/              # Problem sets (pset-01.tex → pset-09.tex)
    └── solutions/                 # Solution write-ups
```

## How to Track Progress

Use GitHub Issues + Milestones + Projects board.

### Labels

| Label | Purpose |
|---|---|
| `notes` | Week 1 self-study tracking |
| `pset` | Week 2 problem set tracking |
| `stuck` | Need help on specific problems |
| `sprint-1` … `sprint-9` | Categorize by sprint |

### Workflow per Sprint

1. **Start a sprint** → Create a Milestone (if not done), then use the templates to create:
   - One issue using `.github/ISSUE_TEMPLATE/notes.md` for Week 1
   - One issue using `.github/ISSUE_TEMPLATE/pset.md` for Week 2

2. **Week 1 checklist** → Open `notes` issue, check off reading/watching/writing notes. Save notes to `real-analysis/notes/sprint-NN-notes.tex`.

3. **Week 2 checklist** → Open `pset` issue, check off each problem as solved. Write solutions in `real-analysis/solutions/pset-NN-sol.tex`.

4. **Mark complete** → Close the milestone when both issues are resolved. Move to next sprint.

### GitHub Project Board

Create a Projects board with columns:
`Backlog → In Progress → Notes Done → PSet In Progress → PSet Done → Complete`

Each Milestone = one Sprint. Issues auto-populate with the right labels.

## Resources Summary

| Sprint | Primary Text | Supplementary |
|---|---|---|
| 1-3 | Abbott Ch. 1-3 | Rudin Ch. 1, Tao's lectures |
| 4-6 | Abbott Ch. 4-6 | Rudin Ch. 2-7 (selective) |
| 7 | Rudin Ch. 6 / Abbott | Tuckerman |
| 8 | Munkowski Ch. 2 | Rudin Ch. 2 gen. |
| 9 | Tao Ch. 11+ | Rudin Ch. 11 (optional) |

## Tips for Success

- **5-8 hours/week**: Pace yourself. Early sprints (especially #1) may take longer as you build proof-writing intuition.
- **Write everything out**: Don't just read — prove every theorem yourself first before looking at solutions.
- **Use the `stuck` label** when you're truly stuck — revisit after 24 hours, then consult hints.
- **Buffer days**: Some sprints may naturally take 3 weeks. That's fine.
