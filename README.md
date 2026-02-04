# DuplicateFileFinder

DuplicateFileFinder is a fast, cross-platform command-line tool that detects duplicate files based on their **exact content**, not just file names.

It works with **any file type**:
- Videos 🎬
- Music 🎵
- Images 🖼️
- Documents (PDF, DOCX, TXT, etc.)
- Archives, executables, and more

If two files have identical content, they will be detected as duplicates — even if they have different names or are located in different folders.

---

## ✨ Features

- Recursive directory scanning
- Content-based duplicate detection (SHA-256)
- Optimized scanning using file size grouping
- Clear, color-coded output:
  - 🟢 Green: file to keep
  - 🔴 Red: duplicate copies
  - 🔵 Helpful suggestions
- Human-readable statistics
- Cross-platform (Windows, Linux, macOS)
- No ads, no tracking, no data sent anywhere

<img width="1737" height="369" alt="DuplicateFileFinder" src="https://github.com/user-attachments/assets/6d3747f3-2886-403c-9324-993d121966c9" />

---

## 🔒 Why this tool is safe and reliable

DuplicateFileFinder does **not** rely on file names, dates, or metadata.

Instead, it uses a **two-step verification process**:

1. **File size grouping**  
   Files with different sizes are automatically excluded (they cannot be identical).

2. **SHA-256 hashing**  
   Files with the same size are verified using the SHA-256 cryptographic hash algorithm.

SHA-256 guarantees that:
- If two files have the same hash, their content is **100% identical**
- False positives are practically impossible

You can safely trust the results.

---

## 🛠️ Technology

- **Language:** Python 3
- **Libraries:** Python Standard Library only
  - `os`
  - `hashlib`
  - `pathlib`
  - `collections`

No external dependencies are required.

---

## 🚀 How to use

### Requirements
- Python 3.8 or newer

### Basic command

```bash
python DuplicateFileFinder.py scan "C:\Path\To\Directory"

