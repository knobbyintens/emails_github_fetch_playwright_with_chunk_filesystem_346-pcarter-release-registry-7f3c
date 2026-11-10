# Release registry

This repository records the release state of the research artifacts produced by
the group. It is the authority for what may be mirrored on the public site.

## How to read it

- `release_manifest.json` is a **quarterly point-in-time snapshot**. It is frozen
  at `generated_at` and is not updated between snapshots, so it lags behind
  reality.
- `status_log.md` is the **append-only live record**. Entries are appended at the
  bottom in chronological order; a later entry supersedes every earlier entry for
  the same project. Read the file to the very end before acting on it.
- The release office also posts one announcement message per event to the shared
  release-announcements mailbox folder. Those messages restate the same live
  facts; the folder is not sorted by topic, so page through it rather than
  assuming the first screen is the whole picture.
- Repository names occasionally change. Resolve the current name from the newest
  status entry and from repository search; never assume an archived name is still
  the artifact.
- An artifact may be linked publicly only when it is owned by this account, the
  current repository is publicly visible, its release state is `public`, and its
  README does not declare a pre-release, embargo or internal state.

Both views are deterministic. If they appear to disagree, it is a staleness or
ordering artefact, not a broken data source: the snapshot was produced at
`generated_at` and the log was appended afterwards. Reconcile against the newest
entries before deciding.

The portfolio site mirrors this registry; it does not maintain its own release
state.
