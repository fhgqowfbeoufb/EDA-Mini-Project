Smart File Organizer
A zero-dependency Python script to categorize files instantly.

Core Features
Automatic Sorting: Groups files into subfolders (Images, Documents, Code, etc.) based on extension.

Dry-Run Mode: Use the --dry-run flag to preview changes without moving any files.

Duplicate Protection: Prevents overwriting by appending timestamps to filenames if a conflict is detected.

Cross-Platform: Compatible with Windows, macOS, and Linux using only the Python standard library.

Usage Instructions
Organize Current Folder: python organizer.py

Organize Specific Folder: python organizer.py /path/to/folder

Preview Changes: python organizer.py --dry-run

Technical Specifications
Language: Python 3.x

Core Modules: os, shutil, sys, datetime

Methodology: Scans directories using os.scandir, maps extensions via a dictionary, and executes moves with shutil.move.

Safety: Uses os.makedirs(exist_ok=True) to ensure destination directories exist before file operations begin.

Future Roadmap
Undo Functionality: Implement a JSON log to track and reverse file moves.

Real-time Monitoring: Integrate the watchdog library to sort files as they are created.

User Interface: Develop a simple graphical folder picker using the Tinker module.
