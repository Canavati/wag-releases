# WhatsApp Agent Gateway releases

Signed releases of WhatsApp Agent Gateway for macOS (Apple silicon). This repo holds only release files; there is no source code here.

Install:

```sh
curl -fsSL https://github.com/Canavati/wag-releases/releases/latest/download/install.sh | sh
```

Every release carries `SHA256SUMS` and `SHA256SUMS.<kid>.sig`, an ECDSA P-256 signature. The installer and the in-app updater refuse anything not signed with a trusted key.

Signing key id: `99e099097c8e021e`

To inspect the installer before running it: download `install.sh`, run `sh install.sh --check`, and confirm it prints `Firma (99e099097c8e021e)`.
