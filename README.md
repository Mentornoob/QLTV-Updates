# QLTV-Updates

Public update metadata for QLTV Desktop.

This repository intentionally contains only release metadata. The main QLTV source code can stay private.

## Files

- `update.json`: Manifest read by QLTV clients.
- GitHub Releases: Public installer files such as `QLTV_Setup_v2.0.2.exe`.

## Release Flow

1. Build the installer from the private QLTV repository.
2. Create a GitHub Release in this repository, for example `v2.0.2`.
3. Upload the installer asset, for example `QLTV_Setup_v2.0.2.exe`.
4. Update `update.json`:

```json
{
  "version": "2.0.2",
  "title": "QLTV 2.0.2",
  "release_date": "2026-07-11",
  "download_url": "https://github.com/Mentornoob/QLTV-Updates/releases/download/v2.0.2/QLTV_Setup_v2.0.2.exe",
  "notes": [
    "Them tinh nang moi.",
    "Sua loi va cai thien hieu nang."
  ]
}
```

5. Commit and push `update.json`.

Clients read:

```text
https://raw.githubusercontent.com/Mentornoob/QLTV-Updates/main/update.json
```
