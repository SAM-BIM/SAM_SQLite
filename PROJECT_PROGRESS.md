# Project Progress - SAM_SQLite (2026-Q4)

## Q4 agent instructions rollout closeout - 2026-10-12

- SAM-BIM/SAM_SQLite#6 merged as `7e45a53dc3a7e3365f01430084c4cd48f45b7326` (merge commit pinned to approved head `fe40b3016a8e96c4e5189da2997fcc43f6bc6dcf`; base `sow/2026-Q4` `b2642239f7267159bdcd5a48ce5e23c17a95e1e7`; validated content `106e9592ed7be26dc218a946effca09a0b1ac6de`). Owner-authorized 2026-10-12 after an independent review (`AGENT_ROLLOUT_REVIEW_2026-10-12.md`, local to the owner's workspace, not committed).
- Docs only: AGENTS.md, CLAUDE.md, plus the rollout record `documentation/Agent-Continuity-Rollout-Q4.md`. No product code, build, workflow, dependency pin or tool changed; this closeout is the only `PROJECT_PROGRESS.md` change.
- Validation: local documentation checks and commands are in `documentation/Agent-Continuity-Rollout-Q4.md` (`git diff --check`, file scope, UTF-8/LF/no BOM, import). Hosted checks at the approved head: spdx success (run 38258082581); build success (run 38258082499). Dependency selection: the build log shows no sibling dependency clones.
- Cleanup: remote docs/agent-instructions-rollout-q4 deleted with an expected-SHA lease on fe40b3016a8e96c4e5189da2997fcc43f6bc6dcf after confirming it is contained in sow/2026-Q4 and no open PR uses it as head or base; the local branch and its worktree are preserved (worktree in use). Other branches, worktrees and the frozen quarters were not touched.
- Remaining gaps: no agent-client behaviour or token benchmark has been run.
- Exact next step: Continue from the shared `AGENTS.md`. Open item carried from the pilots: verify on each installed agent client, in a fresh Q4 session, that it follows the instructions without loading the full progress history, and record the result.

## Branch

`sow/2026-Q4` - bootstrapped 2026-10-06 from `master` `80ab3b68`. Frozen Q3 record: `sow/2026-Q3` @ `c2b56f1e` (not modified).

## Last updated

2026-10-06 (Q4 operational cleanup).

## Current status

Q4 branch cut from `master` `80ab3b68`, which is the exact commit pinned in SAM_Deploy's frozen Q3 baseline (`v20261006.1`). Bootstrap added only internal docs (this file, `AGENTS.md`). No product source changed. No Q4 product work has started.

## Q4 priorities

Not yet set by the owner. Record them here at the first Q4 planning pass. Known carry-over work is listed below.

## Known carry-over work

- None identified for this repository at bootstrap.

## Repository-specific next steps

- Await Q4 planning. Open PRs for Q4 work against `sow/2026-Q4`.
- Follow the continuity convention in `AGENTS.md` for every PR and closeout.

## Decisions / assumptions

- Q4 base is `master` `80ab3b68`; the internal files were recovered from `sow/2026-Q3` into this branch only, never onto `master`.
- Q4 history intentionally does not contain the Q3 branch history (the maintained `master` is the promoted Q3 line, which is not a descendant of `sow/2026-Q3`); the frozen `sow/2026-Q3` branch is the permanent record.
- Historical Q2/Q3 content below is kept as evidence; its branch names, SHAs and next steps describe Q3 and are not current instructions.

## Validation

- Bootstrap verified 2026-10-06: `sow/2026-Q4` was created at exactly `80ab3b68` and the push was a normal (non-forced) branch creation.

## Issues / blockers

- None at bootstrap.

## Next step

- Owner to set Q4 priorities; then start the first Q4 task from this branch.

## Q4 operational cleanup (2026-10-06)

- Reviewed every active Q2/Q3 reference in this repository on `sow/2026-Q4` (workflow branch filters, dependency-branch resolution, `.gitmodules`/validation, docs). Historical Q2/Q3 mentions (feature documentation records, the frozen Q3 section below) are intentionally unchanged.
- Changed (`913a24e`): removed the dead `$candidates += 'sow/2026-Q2'` fallback from the dependency-branch resolution in `.github/workflows/build.yml`. No dependency repository has a `sow/2026-Q2` branch, so the entry never matched and resolution already fell through to the default branch; behaviour is unchanged (PR head ref, current sow ref, then the dependency's default branch) and no per-quarter edit is needed.
- Checked, no action: the `github.repository_owner == 'SAM-BIM'` build guard (intentional; its comment names HoareLea only to explain why the guard exists), CODEOWNERS (SAM-BIM owners), and workflow secrets (no HoareLea-named secret). The local `upstream` (HoareLea) remote is preserved.
- Full cross-repository record, migration table and owner decisions: `SAM_Deploy:sow/2026-Q4` `PROJECT_PROGRESS.md`.

---

# Historical record - 2026-Q3 (frozen)

Source: last revision of the file on `sow/2026-Q3`, commit `7bc76f2` (the file was removed from the Q3 tip by `c2b56f1`; `sow/2026-Q3` tip is `c2b56f1e`). The Q3 file was an unpopulated template ("Not updated yet"); no Q3 work was recorded in this repository's progress file.
