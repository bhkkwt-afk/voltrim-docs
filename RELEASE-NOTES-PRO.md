## Voltrim FlipCraft Pro — v1.0.0

Create stunning interactive flipbooks from PDFs, photos, and Word documents —
with built-in content encryption to protect your work.
One payment of $29. No subscription. No watermarks. No page limits. Forever yours.

---

### What's Included in This Release

| File | Description |
|------|-------------|
| `VoltrimFlipCraftPro-Setup-1.0.0.zip` | Installer ZIP — extract and run the .exe inside |
| `VoltrimFlipCraftPro-Setup-1.0.0.zip.sha256.txt` | SHA256 checksum for verifying your download |

---

### Features

**Four Creation Modes**
- 📄 PDF Flipbooks — import any PDF at Screen (96 DPI), Standard (150 DPI), or High (300 DPI) quality
- 🖼️ Image Album mode — JPG, PNG, and WEBP image folders into photo flipbooks
- 📝 Word Document mode — .docx and .doc files via Microsoft Word or free LibreOffice
- 🔗 Multi-Document Merge mode — combine multiple PDFs and Word docs into one flipbook

**Viewer & Output**
- Native Windows viewer output (.exe + .dat encrypted pair)
- Smooth 3D page-flip animations with sound effects
- Book opening and closing animations
- Progress bar with draggable scrubber
- Fullscreen mode, zoom controls, and keyboard navigation
- Sound on/off toggle
- Professional 3D front and back cover page generation

**Protection & Privacy**
- Built-in content encryption — unique XOR key per flipbook
- Encrypted .dat content file — unreadable without the matching .exe
- Content decrypted only at runtime into a hidden temporary folder
- Temporary folder deleted automatically when viewer closes
- No HTML files or images exposed in the output folder
- 100% offline after first setup — no cloud, no accounts, no telemetry

**No Restrictions**
- No page limits — create flipbooks of any size
- No watermarks — ever
- No limit on how many flipbooks you can create
- One licence — one payment — unlimited use

---

### System Requirements

- Windows 10 or Windows 11 (64-bit)
- .NET Framework 4.5 or later (pre-installed on all modern PCs)
- Internet required on first launch only (~25 MB Poppler download, one-time)
- Internet required on first flipbook creation only (~4 MB WebView2 libraries, one-time)
- Word Document mode: Microsoft Word or free LibreOffice

---

### How to Install

1. Download `VoltrimFlipCraftPro-Setup-1.0.0.zip`
2. Extract the ZIP to a folder on your computer
3. Read `READ_ME_FIRST.txt` before proceeding
4. Double-click `VoltrimFlipCraftPro-Setup-1.0.0.exe`
5. If Windows SmartScreen shows a warning — click **More info** then **Run anyway**
6. Follow the installation steps and click Finish

---

### Verify Your Download (Optional but Recommended)

To confirm your download is genuine and was not corrupted, open
PowerShell and run:

```powershell
Get-FileHash "VoltrimFlipCraftPro-Setup-1.0.0.zip" -Algorithm SHA256
```

Compare the result against the hash in
`VoltrimFlipCraftPro-Setup-1.0.0.zip.sha256.txt` included in this
release. They must match exactly.

---

### About the Two-File Flipbook Output

Every flipbook you create with FlipCraft Pro produces two files:

- `[Title].exe` — the viewer application (contains the unique decryption key)
- `[Title].dat` — the encrypted flipbook content (unreadable without the .exe)

Both files must always stay in the same folder.
Double-click the `.exe` to open the flipbook instantly.

When sharing your flipbook with others, always deliver both files together
by email, Google Drive, USB drive, or any file-sharing platform.
Recipients only need Windows 10 or Windows 11 — no installation required on their end.

---

### First Launch Notes

**Poppler PDF Engine (~25 MB)**
On first launch, FlipCraft Pro automatically downloads the Poppler PDF
rendering engine from GitHub. This is a one-time download. An internet
connection is required for this step only. After this, the app works
completely offline.

**WebView2 Viewer Libraries (~4 MB)**
On your first flipbook creation, FlipCraft Pro downloads the Microsoft
WebView2 display libraries from NuGet. This is also a one-time download.
All subsequent flipbook creation works fully offline.

---

### Documentation

Full documentation is available in the `docs` folder included with
the installer and in the GitHub repository:

| Document | Description |
|----------|-------------|
| `README.txt` | Overview and quick start guide |
| `INSTALLATION-GUIDE.txt` | Detailed installation and first-run instructions |
| `CHANGELOG.md` | Full version history |
| `EULA.txt` | End User Licence Agreement |
| `PRIVACY-POLICY.txt` | Privacy policy |
| `SECURITY.md` | Security architecture and vulnerability reporting |
| `THIRD-PARTY-NOTICES.txt` | Open-source component credits |

---

### Support

📧 voltrimcreativeminds@gmail.com
🌐 https://voltrim-flipcraft-pro.netlify.app
📦 https://github.com/bhkkwt-afk/voltrim-docs/releases/latest

© 2026 Voltrim Creative Minds
