# claude-md

My global `CLAUDE.md` for [Claude Code](https://claude.com/claude-code): the rules that
are loaded into every session, in every project.

## What it sets up

- **Orchestrate, delegate, review.** The main session plans and reviews. Coding goes to
  a `coder` subagent, research to a read-only `researcher` subagent, and trivial edits
  stay inline.
- **Think before delegating.** State assumptions, prefer an existing tool over new code,
  re-plan after two failed attempts.
- **Simplicity and surgery.** Minimum code, touch only what the request needs.
- **Verification.** Turn tasks into checks that can be run, and see the output before
  calling something done.
- **Defaults** for ambiguous wording, context efficiency, git hygiene and capturing
  lessons after a correction.

## Use

Copy `CLAUDE.md` to `~/.claude/CLAUDE.md`.

The file refers to things that are not in this repository. Supply your own or delete the
references:

- `coder` and `researcher` subagent definitions (`~/.claude/agents/`)
- `~/.claude/checklists/pre-review.md`, the checklist the reviewer reads

## License

GPL-3.0-or-later. See [LICENSE](LICENSE).
