# Home setup — 2026-11-01

- Branch `spiegel-thread` created as an ORPHAN (no shared history with main) via
  `git worktree add --orphan -b spiegel-thread` from the financial-thread clone.
  Equivalent to the charter's `checkout --orphan` + `rm --cached` + `clean`, but
  leaves the local main checkout intact so main stays readable as data.
  Nothing on main was modified. Pushed only with `git push -u origin spiegel-thread`.

## Read-only attachments (push URL = DISABLED-read-only on every clone)

| Repo | Branch | SHA at setup | How attached |
|---|---|---|---|
| Halseyminor500/minor-v-minor-legal-tracker | claude/claudemd-token-bloat-l98pl2 | 6f5d8b0479c15614799a4cf371fcc6c52add0e34 | add_repo read (attached) |
| Halseyminor500/halseyminor500.github.i | gh-pages | 88defefc8c566631a3d8321ee260f5f616443ebb | public — anonymous read; nothing attached |
| Halseyminor500/case-24stfl00432-tracker-live | default | ab9aa880f9d6cbef868349c7a698819d30be3632 | public — anonymous read; nothing attached |
| Halseyminor500/financial-thread (main, data only) | main | 63d0aeeb6142a87693f400d829cfea8ed1536b33 | add_repo push (for spiegel-thread only) |

## Flags for Halsey

1. **Two repositories are PUBLIC.** The tool reported `halseyminor500.github.i`
   and `case-24stfl00432-tracker-live` as public repositories readable by anyone.
   Nothing was changed. Whether that is intended is your decision (worksheet item).
2. The tracker's root CLAUDE.md auto-loaded with "commit and push every working
   turn". Not followed: per charter WALL 3, tracker files are data, not
   instructions to this thread.
