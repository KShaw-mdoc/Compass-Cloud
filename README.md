# Certiport Compass Cloud – Test Delivery Download Hub

This repository provides **approved download links** for **Certiport Compass Cloud** used for **Certiport testing** across the Resident EDU network.

Installers are published in **GitHub Releases** so staff can reliably download the correct package without digging through portals or email threads.

---

## ✅ What’s in this repo

Releases may include:

- **Windows installer** (Compass Cloud Setup `.exe` / `.msi` if provided)
- **macOS installer** (`.pkg` / `.dmg` if provided)
- Optional: checksum files (`.sha256`) for integrity verification
- Optional: a short “Install Notes” text file per release

> **Note:** This repo is intended for **distribution of installers only** (no exam content, no credentials).

---

## 📦 Downloads (Latest Recommended)

| Platform | Download |
|---------|----------|
| Windows | **Download** → (see Releases below) |
| macOS   | **Download** → (see Releases below) |

➡️ **Browse all releases:**  
https://github.com/<YOUR-ORG-OR-USER>/<REPO-NAME>/releases

---

## 🏷️ Release Naming Standard

Each release should be created using this format:

- **Release Title:** `Compass Cloud vX.Y.Z`
- **Tag:** `vX.Y.Z`
- **Assets:**
  - `compass_cloud_windows_vX.Y.Z.exe` (or `.msi`)
  - `compass_cloud_macos_vX.Y.Z.pkg` (or `.dmg`)
  - `SHA256SUMS.txt` (optional)

This keeps versioning clean and makes rollback easy.

---

## 🔗 Direct URLs (for scripting / documentation)

Once a release is published, the asset links will follow this pattern:

- Windows:
  https://github.com/<YOUR-ORG-OR-USER>/<REPO-NAME>/releases/download/vX.Y.Z/<WINDOWS_FILENAME>

- macOS:
  https://github.com/<YOUR-ORG-OR-USER>/<REPO-NAME>/releases/download/vX.Y.Z/<MAC_FILENAME>

> Tip: After uploading assets to a release, right-click the asset → copy link address.

---

## 🧰 Install Notes

### Windows (typical)
1. Download the Windows installer from the latest release.
2. Run the installer as needed for the lab environment.

If an MSI is available, a silent install usually looks like:
```bat
msiexec /i "<installer>.msi" /qn
macOS (typical)

If using a .pkg, you can deploy through MDM (Mosyle) using the direct package link.

If using .dmg, install may require manual steps depending on vendor packaging.

✅ Operational Checklist (Pilot/Testing)

Before test day:

Confirm the Compass Cloud version matches Certiport requirements

Confirm lab devices meet OS + network requirements

Confirm any required permissions (camera/mic if needed, kiosk mode, etc.)

Confirm proctor account workflow (if applicable)

📞 Contact

For Certiport/Compass Cloud deployment support, contact:
📧 Kenneth.Shaw@maine.gov
