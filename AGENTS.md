# Shopwell repository rules

This repository is the independently maintained Shopwell project template.

- Preserve UTF-8 and existing user changes.
- The project and its Composer manifest use the Apache License 2.0 (`Apache-2.0`); root `LICENSE` contains the standard text.
- Preserve every upstream legal text verbatim in root `NOTICE`.
- Outside `NOTICE`, do not reintroduce Shopware branding, package names, repositories, or Actions.
- Composer dependencies must use stable versions from a real registry. Git URLs, branches, commits, `dev-*`, `path`, `file`, and `link` fallbacks are not releases.
- Do not merge or cherry-pick unrelated upstream history, copy upstream tags, or force-push.
- Before commit, push, release, or sync completion, run:
  `../sync-upstream/bin/syncctl audit-license template` and
  `../sync-upstream/bin/syncctl audit-upstream-dependencies template`.
- A failed audit blocks completion.
