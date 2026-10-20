# Changesets

Every PR that changes the published package needs a changeset, which becomes the release note in `CHANGELOG.md`.

CI only requires it when the PR changes the published code (`index.js`, `index.d.ts`, `configs/` or `lib/`, see `changedFilePatterns` in `config.json`).
It does not detect changes of `package.json`: add a changeset yourself when changing `dependencies`, `peerDependencies` or `engines`.

```sh
pnpm changeset          # choose major / minor / patch and write the summary
pnpm changeset --empty  # for a PR that should not appear in the release notes (CI, docs, ...)
```

See [the Changesets docs](https://github.com/changesets/changesets/blob/main/docs/adding-a-changeset.md) for details.
