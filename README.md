# brik64-dist-releases

Official compiler releases for `brikc` — the BRIK-64 self-hosting toolchain.

🌐 [brik64.dev](https://brik64.dev) · 📖 [docs.brik64.dev](https://docs.brik64.dev)

## Install

```bash
curl -fsSL https://brik64.dev/install | sh
```

Or download from [Releases](https://github.com/brik64/brik64-dist-releases/releases).

## Verify

```bash
brikc --version
# brikc v2.0.0 (fixpoint: 7229cfcd...)

brikc check --self
# ✓ Self-compilation fixpoint verified
# ✓ Hash: 7229cfcde9613de42eda4dd207da3bac80d2bf2b5f778f3270c2321e8e489e95
```

## Release Integrity

Every binary is:
- SHA256 checksummed (`SHA256SUMS`)
- SLSA provenance attested
- Cosign signed via Sigstore

```bash
cosign verify-blob brikc-linux-x86_64 \
  --signature brikc-linux-x86_64.sig \
  --certificate brikc-linux-x86_64.pem
```

## Platforms

| Platform | Binary |
|----------|--------|
| Linux x86-64 | `brikc-linux-x86_64` |
| macOS arm64 | `brikc-darwin-arm64` |
| macOS x86-64 | `brikc-darwin-x86_64` |

## License

© 2026 BRIK-64 Inc. All rights reserved. Proprietary license.
Binaries are provided for use only — redistribution is prohibited without written permission.
