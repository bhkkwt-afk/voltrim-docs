# Voltrim FlipCraft — Security Policy

Copyright © 2026 Voltrim Creative Minds

---

## Supported Versions

| Version | Supported |
|---------|-----------|
| 1.0.x   | ✅ Yes    |

---

## Reporting a Vulnerability

If you discover a security vulnerability in Voltrim FlipCraft, please report
it responsibly by emailing: **voltrimcreativeminds@gmail.com**

Please include:
- A description of the vulnerability
- Steps to reproduce the issue
- The version of Voltrim FlipCraft affected
- The edition (Basic or Pro) affected
- Any proof-of-concept code or screenshots (if applicable)

We will respond within 5 business days and aim to release a patch within
30 days of a confirmed vulnerability.

**Please do not disclose vulnerabilities publicly until a fix is available.**

---

## Security Architecture

### Content Protection (Pro edition)

- Each flipbook is encrypted with a unique 32-character alphanumeric XOR key.
  The key is generated randomly at creation time and embedded in the viewer exe.
- The encrypted content file (.dat) is unreadable without the matching .exe.
- Content is decrypted only in memory and into a hidden temporary system folder
  at runtime. The temporary folder is deleted automatically when the viewer closes.
- No HTML files, image folders, or readable source content are present in the
  output folder.

### Network Security

- Voltrim FlipCraft does not transmit your PDFs, images, documents, or
  generated flipbook content to any server.
- All PDF rendering and flipbook creation is performed entirely on your PC.
- The only outbound network requests made by the application are:
    (a) Downloading Poppler from GitHub on first launch (one-time, ~25 MB)
    (b) Downloading WebView2 DLLs from NuGet on first Pro flipbook creation
        (one-time, ~4 MB, stored in user AppData)
    (c) Checking for Poppler updates when you click Check Updates
- Generated flipbook viewer executables make no network requests.

### Viewer Security

- The Pro edition viewer runs Microsoft WebView2 in a restricted context:
    - Context menus are disabled
    - Developer Tools are disabled
    - Status bar is disabled
    - Zoom control is disabled
- These restrictions prevent easy inspection or extraction of flipbook content.

### Privacy

- The application collects no personal data, usage statistics, or telemetry.
- No user accounts are required or created.
- All generated content remains entirely on your computer.
- See PRIVACY-POLICY.txt for the full privacy policy.

---

## Contact

Security issues: voltrimcreativeminds@gmail.com
Website: https://voltrim-flipcraft.netlify.app
