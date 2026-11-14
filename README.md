# Trivy — TrillionAI Engineering Reference

**Research-only source archive for TrillionAI Audit. Not a production TrillionAI service.**

## Upstream source

- Official upstream: https://github.com/aquasecurity/trivy
- Pinned upstream commit: `239be7b2671a3c9706bbfec2ba4677210cbdcdec`
- Expected upstream root Git tree: `2a1dae04bf06b3b5d9cb01e9c4a97f7bfbe178a0`
- Source snapshot branch: `trivy-upstream-snapshot`
- Archived source directory: `upstream/` **(imported and verified)**
- Root upstream licence: **Apache License 2.0** (original licence retained inside the source snapshot)
- GitHub source inventory at the pinned commit: 5,062 Git tree entries (including directories); 95,609,909 bytes of tracked blob contents.

## Source import and verification

**Verified: GitHub Actions source-import job passed.**

- [Successful source import and integrity verification](https://github.com/Anselm04/Trivy-Source-Code-Reference/actions/runs/43644568008)
- Verified filtered remote source Git tree: `46aa6ce270ab851890ec427ccfb4881f03293f81`
- Snapshot branch contains **4,994 upstream Git tree entries**, including directories.
- Retained **3,387 tracked blobs** (~95.5 MB by GitHub's blob-size inventory).
- Original pinned upstream Git tree: `2a1dae04bf06b3b5d9cb01e9c4a97f7bfbe178a0` (before exclusions).
- **Excluded:** 66 files in `pkg/fanal/secret/testdata/` and `pkg/fanal/artifact/local/fs_test.go`. GitHub push protection flagged credential-shaped test fixtures in these paths. The exclusions were deliberate; **the filtered snapshot is NOT a byte-for-byte full copy of the unfiltered upstream tree**.

The [import workflow](.github/workflows/import-trivy-source.yml) retrieves the pinned Git revision without running Trivy, imports the exact Git tree under `upstream/` on a separate branch, and compares the fetched/pushed `upstream/` tree to the expected upstream tree hash.

**Verification status: source snapshot imported and its filtered Git tree verified against the pinned source with declared exclusions.** This does not prove runtime tests pass or that excluded test fixtures are available.

Once verified, browse:
[Trivy source snapshot](https://github.com/Anselm04/Trivy-Source-Code-Reference/tree/trivy-upstream-snapshot/upstream).

The archive includes tracked test fixtures and upstream attribution. It does not contain upstream Git commit history, unrelated deployment infrastructure, or separately downloaded Git LFS contents/submodule contents. The imported Git tree is a pinned snapshot, not necessarily the latest Trivy release.

## Research for TrillionAI Audit

Study original Trivy implementations for:
- Dependency and OS vulnerability checks
- Source and image misconfiguration analysis
- Secrets detection and evidence redaction
- Software licence risk assessment
- Scanner output normalisation and machine-readable findings
- Version pinning, vulnerability database provenance and safely bounded execution

Keep the upstream source separately from proprietary TrillionAI Audit code. Implement original Node.js/TypeScript integration interfaces and Flutter views, with independent tests and auditable verification evidence. Do not import the entire Trivy codebase into the private product.

## Licensing and provenance

The upstream Trivy source is copyrighted by Aqua Security and contributors under their applicable licences. Retain upstream licence and copyright text; check subdirectories and bundled third-party components before distributing or incorporating any individual file. This research repository does not relicence third-party code.

No paid infrastructure or TrillionAI product deployment is activated by this source import.
