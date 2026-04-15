# Xp3Extractor
XP3 Visual Extractor A fast, multi-threaded Windows GUI tool for extracting files from XP3 archives, commonly used in visual novels powered by the Kirikiri engine.
✨ Features
Simple GUI – Built with native Win32 API, no external UI frameworks required.

Multi-threaded Extraction – Utilizes all CPU cores for maximum performance on large archives.

Full XP3 Support – Handles both compressed (zlib) and uncompressed segments.

Robust Encoding Handling – Correctly preserves Japanese/Chinese filenames via UTF‑16LE → UTF‑8 → ANSI conversion.

Error Resilient – Continues extraction even if some files fail, with a detailed summary report.

Large File Optimized – Uses chunked reading for uncompressed data to keep memory usage low.

Portable – Single executable with no installation required.
📦 How It Works
The tool reads the XP3 index (optionally compressed), parses file entries and their segments, then concurrently writes extracted files to an output folder named <archive>_extracted. A built-in log window shows real‑time progress.

🚀 Usage
Download the latest release from the Releases page.

Run XP3_Extractor.exe.

Click "Select XP3 File and Extract..." and choose your .xp3 archive.

Wait for the extraction to complete – a message box will appear when done.

Find the extracted files in the automatically created *_extracted folder next to the archive.

🔧 Building from Source
Requirements
Windows SDK (comes with Visual Studio or MinGW‑w64)

C++11 compatible compiler

The single‑file miniz.c library (already included)
