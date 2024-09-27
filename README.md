
# Automation & Python - Organizing Files

This Python script automates the organization of files in your macOS Downloads folder. It moves files into categorized subfolders based on their file types, keeping your Downloads folder tidy and organized.

### Features:
- **Automation with Python**: Automatically sorts downloaded files into predefined folders based on file extensions.
- **File Type Sorting**: For example, if an image file like `demo.jpg` is downloaded, the script moves it to `Downloads/images`. Similarly, `.docx`, `.pdf`, and `.txt` files are moved to `Downloads/documents`, and other file types follow the same logic.

### Folder Organization:
- **Images**: `.jpg`, `.png`, etc.
- **Documents**: `.docx`, `.pdf`, `.txt`, etc.
- **Softwares**: Application and installation files.
- **Others**: Files that don't fit the above categories.
- **Logs**: A dedicated log folder to track script operations, including a `log.txt` file.

### Technical Overview:
- **os module**: Facilitates interaction with the operating system, allowing access to the file system for tasks like identifying and moving files.
- **shutil module**: Provides higher-level file operations, such as copying, moving, and deleting files.

### Prerequisites:
1. Ensure Python 3 is installed on your system.
2. Place the script (`automation.py`) in the Downloads folder.
3. Create the following folders within the Downloads directory:
   - `images/`
   - `documents/`
   - `softwares/`
   - `others/`
   - `Log/` (This folder will contain a `log.txt` file where the script logs its output.)

### How to Run:
1. Open Terminal and navigate to your Downloads folder:
   ```bash
   cd ~/Downloads
   ```
2. Run the script:
   ```bash
   python3 automation.py >> ~/Downloads/Log/log.txt
   ```

### Automating with Cron:
To run the script automatically at specified intervals, you can set up a cron job. Follow the instructions in `cronjob.md` or refer to this [article](https://medium.com/swlh/automation-python-organizing-files-5d2b6b933402?source=friends_link&sk=da95bd01abb41776dd9230a72ba8f193) for detailed steps.
