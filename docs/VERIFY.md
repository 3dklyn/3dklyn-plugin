# Verify the personal beta download

Release: **1.34.27 · Build 97**

File: `3DKLYN-personal-beta-1.34.27.mzp`

SHA-256:

```text
34cb19a4138860d81cda050846196ac9965fc413d6a99ebd497fb4e82caf6657
```

The same checksum is published independently on the [official website](https://3dklyn.com/verification.html).

In PowerShell, replace the example path with the location of your download:

```powershell
Get-FileHash -Algorithm SHA256 -LiteralPath 'C:\path\to\3DKLYN-personal-beta-1.34.27.mzp'
```

Compare the complete value. If it differs, do not install that copy; download it again from the official release or website.

The MZP is unsigned. A checksum verifies matching bytes, not a publisher certificate. A checksum supplied only alongside an untrusted archive does not independently establish its source. The archive's per-file integrity manifest is also not a digital signature.

The GitHub release contains the unchanged installer distributed at [3dklyn.com](https://3dklyn.com/downloads/3DKLYN-personal-beta-1.34.27.mzp).
