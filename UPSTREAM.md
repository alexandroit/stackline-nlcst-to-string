# Upstream and maintenance review

This package maintains `nlcst-to-string@3.1.1` under the independent `@stackline/nlcst-to-string` name.

- Source: https://github.com/syntax-tree/nlcst-to-string/tree/6f915c28d57119847086e1e479ae789dcef9f962
- Public npm artifact integrity: `sha512-63mVyqaqt0cmn2VcI2aH6kxe1rLAmSROqHMA0i4qqg1tidkfExgpb0FGMikMCn86mw5dFtBtEANfmSSK7TjNHw==`.
- Upstream issue evidence checked: 2026-09-29T00:22:11.089670+00:00.
- Original license and author notices are retained.
- The upstream published runtime files and declarations are hash-checked in `.stackline/upstream.json`. Any runtime fix is explicitly listed there.
- Functional upstream suites run against the source and extracted final package. Development tools were reduced to those used by validation; full source and runtime audits must pass.
- Only direct dependencies of the original Stackline portfolio are in this migration. This is not a claim that all transitive projects are maintained by Stackline.

## Issue triage

The queried open-issue list contained no issue entries. This does not establish that the upstream is abandoned or bug-free. No runtime bug fix is claimed for this initial maintenance release.

The evidence query fetched the latest 100 open and 30 closed issue/PR entries and removed PRs. Closed entries were collected for context; this report does not claim an exhaustive historic review.

## Release discipline

The source commit, passing CI and CodeQL, reviewed CI tarball hash, npm provenance, normal and aliased installs, and immutable GitHub release are checked before a release is complete. Published versions and tags are never replaced.
