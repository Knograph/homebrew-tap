# Homebrew tap for Kno

[Kno](https://github.com/knograph/kno) measures the marginal value of data
assets for LLM agents — which of your data earns its place in context, RAG,
or a fine-tuning set, what it costs, and what to stop dumping into JSONL.

This repository is the [Homebrew tap](https://docs.brew.sh/Taps) that
`brew install knograph/tap/kno` reads from. It contains exactly one formula
(`Formula/kno.rb`), updated automatically by
[goreleaser](https://github.com/knograph/kno/blob/main/.goreleaser.yaml)
on every release.

## Install

```sh
brew tap knograph/tap
brew install kno
```

Verification before installing is the same as the
[release notes](https://github.com/knograph/kno/releases) describe: every
release ships a `checksums.txt`, a keyless cosign bundle over it, an SPDX
SBOM per archive, and SLSA build provenance. Homebrew itself verifies the
formula's pinned SHA-256 on download.

## Uninstall

```sh
brew uninstall kno
brew untap knograph/tap
```

## Reporting issues

Bugs belong in the main repository: <https://github.com/knograph/kno/issues>.
This repository is machine-maintained — do not open issues or PRs here.
