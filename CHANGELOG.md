# Voltrim FlipCraft — Changelog

All notable changes to Voltrim FlipCraft are documented in this file.
Format follows [Keep a Changelog](https://keepachangelog.com/en/1.0.0/).

---

## [1.0.0] — 2026

### Added — Basic Edition
- PDF to interactive flipbook conversion using Poppler (pdftoppm)
- Native Windows viewer executable (.exe) output
- Encrypted content file (.dat) paired with viewer — content protected
  from extraction or copying
- 3D hard-cover book scene on launch with realistic cover art
- 3D back cover scene after last page
- Realistic page-flip animation with canvas-based 3D effect
- Book opening and closing animations with sounds
- Page-flip sound on every turn
- Sound on/off toggle button
- Zoom in/out controls
- Fullscreen mode
- Progress bar with draggable scrubber and animated page-number label
- Navigation arrows (< >) at stage sides
- Page counter in toolbar
- Three quality settings: Screen (96 DPI), Standard (150 DPI), High (300 DPI)
- Poppler PDF engine auto-download on first run
- Check Updates button for Poppler engine updates
- Open Folder button after flipbook creation
- Create Another button for rapid workflow
- User Manual (HTML, opens in browser)
- Exit button with confirmation dialog
- Activity log panel showing conversion progress and build status
- Output folder selector

### Added — Pro Edition
- All Basic features
- Image Album mode — create flipbooks directly from JPG/PNG image folders
- Word Document mode — import .docx/.doc files via Microsoft Word or
  LibreOffice, converted automatically to PDF then to flipbook
- Multi-Document Merge mode — combine multiple PDFs and Word documents
  into a single unified flipbook in any order
- Native WebView2-powered viewer executable (no browser required)
- Context menu, DevTools, and status bar disabled in viewer
- WebView2 DLLs automatically downloaded from NuGet on first build
- Professional cover page auto-generation for all creation modes

### Security
- Per-flipbook unique XOR encryption key (alphanumeric, 32 characters)
- Content packaged as encrypted .dat file — unreadable without matching .exe
- Decryption occurs in a hidden temporary folder at runtime only
- Temporary folder is deleted automatically when the viewer is closed
- No HTML files or image folders exposed to end users

### Technical
- Pure PowerShell + Windows Forms — no .NET SDK required
- C# compiled at runtime using csc.exe (.NET Framework 4.x)
- csc.exe located automatically from system .NET Framework installation
- WebView2 DLLs resolved by full path at compile time (no short names)
- Alphanumeric-only encryption keys — safe in PowerShell here-strings
- All page images processed as PNG via Poppler pdftoppm
- Poppler PDF engine (pdftoppm + pdfinfo) for accurate rendering
- Supports PDFs of any size and page count — no page limit
- APPDATA used for WebView2 tools folder (no admin rights required)

---

## Roadmap

### Planned — v1.1.0
- Password-protected PDF support
- Custom cover image upload option
- Table of contents / bookmarks panel
- Mobile-responsive viewer layout

### Planned — v2.0.0
- True native rendering — no browser engine required
- Pure Windows GDI+/WPF page rendering
- Smallest possible output file size
- Fastest launch time
