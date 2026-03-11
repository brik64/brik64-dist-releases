# BRIK-64 Distribution

Binary releases for the BRIK-64 compiler (`brikc`).

## Install

```sh
curl -fsSL https://badge.brik64.dev/dist/install.sh | sh
```

**Linux x86-64 only.** Requires `curl` and `sha256sum`.

## Manual download

| File | Description |
|------|-------------|
| [`brikc-v2.0.0`](https://badge.brik64.dev/dist/brikc-v2.0.0) | Compiler ELF (Linux x86-64) |
| [`install.sh`](https://badge.brik64.dev/dist/install.sh) | Installer script |
| [`SHA256SUMS`](https://badge.brik64.dev/dist/SHA256SUMS) | Checksums |

## Verify

```sh
echo "eb3e66023972f08084ed7bb742472d276950cd053b73066aa444c41cce7878cb  brikc-v2.0.0" | sha256sum -c
```

## Releases

Binaries are served via [badge.brik64.dev](https://badge.brik64.dev) — private R2 bucket, rate-limited.

© 2026 BRIK-64 Inc.
