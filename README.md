📂 Smart File Organizer
A zero-dependency Python script to categorize files instantly.

🚀 Features
Auto-Sort: Groups files (Images, Docs, Code, etc.) into subfolders.

Dry-Run: Use --dry-run to preview changes without moving files.

Safe: Renames duplicates with timestamps (no overwriting).

Portable: Works on Windows, Mac, and Linux using only standard libraries.

💻 Usage
Current Folder: python organizer.py

Specific Folder: python organizer.py /path/to/folder

Preview Only: python organizer.py --dry-run

🛠️ Technical Specs
Language: Python 3.x

Modules: os, shutil, sys, datetime

Logic: Uses a dictionary to map extensions to 9+ categories.

Safety: os.makedirs(exist_ok=True) ensures folders exist before moving.

🔮 Future Ideas
Undo: Log moves to a JSON file to reverse sorting.

Watchdog: Auto-sort files the moment they land in Downloads.

GUI: Add a simple "Select Folder" button using Tkinter.
