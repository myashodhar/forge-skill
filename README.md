# forge-skill

A Claude Code skill that eradicates vibe coding by forcing developers to genuinely understand what they are building — before and during implementation.

## What it does

`/forge` activates an uncompromising technical mentor mode:

- **Grills you on prerequisites** before writing a single line of code
- **Teaches from first principles** (Problem → Concept → Mechanism → Implementation) when you have gaps
- **Makes you diagnose your own errors** during implementation — model explains, but only after you try
- **Closes with a debrief** — explain what you built end-to-end before the session ends
- **Persists sessions** so you resume where you left off

## Install

```bash
npx skills add myashodhar/forge-skill@forge
```

## Usage

```
/forge         # Hard mode (default) — root cause understanding required
/forge easy    # Easy mode — mechanical understanding required
```

## Modes

| Mode | Error understanding required | Prereq depth |
|------|------------------------------|--------------|
| Hard (default) | Root cause, bit-level if needed | Full abstraction ladder |
| Easy | Mechanical (one layer above surface) | Full abstraction ladder |

## How it works

1. You describe your project and declare your stack
2. Model builds a prerequisite map as an abstraction ladder
3. Model grills you node by node — pass fast if you know it, get taught if you don't
4. Once all prereqs pass, implementation begins
5. Every error: you diagnose first, model explains in full, then fix proceeds
6. On completion: you explain the system end-to-end, model closes gaps

## License

MIT
