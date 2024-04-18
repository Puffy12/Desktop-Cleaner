# Desktop Cleaner

Desktop Cleaner is a Python script designed to organize files on your desktop by moving them to specific folders based on their file extensions. It utilizes the Watchdog library to monitor the Desktop directory for any file modifications, such as creations or modifications, and then automatically sorts these files into designated folders.

## Installation

1. Clone the repository:

    ```bash
    git clone https://github.com/Puffy12/Desktop-Cleaner.git
    ```

2. Navigate to the project directory:

    ```bash
    cd desktop-cleaner
    ```

3. Create and activate a virtual environment:

    ```bash
    python -m venv .venv
    source .venv/bin/activate    # On Linux/Mac
    .venv\Scripts\activate       # On Windows
    ```

4. Install dependencies:

    ```bash
    pip install -r requirements.txt
    ```

## Usage

1. Make sure you have Python 3 installed on your system.

2. Run the script:

    ```bash
    python desktop_cleaner.py
    ```

3. The script will start monitoring your Desktop directory. Any files created or modified will be automatically moved to appropriate folders based on their extensions.

## Configuration

You can customize the behavior of the script by modifying the following variables in the `desktop_cleaner.py` file:

- `watch_path`: The directory to monitor (by default, it's set to the user's Desktop directory).
- `destination_root`: The root directory where files will be organized.
- `extension_paths`: A dictionary mapping file extensions to their corresponding destination folders.

## Supported Extensions

The script currently supports the following file extensions:

- `.txt`: Text files
- `.pdf`: PDF documents
- `.jpg`, `.png`, `.gif`: Image files
- `.docx`, `.xlsx`, `.pptx`: Microsoft Office files

Feel free to add more extensions and customize the destination folders according to your needs.

## Library Imports

The script utilizes the following Python libraries:

- `watchdog`: A library for monitoring file system events.
- `shutil`: A module for high-level file operations.
- `datetime`: A module for manipulating dates and times.
- `pathlib`: A module for representing file paths.
- `FileSystemEventHandler`: A class from the `watchdog.events` module for handling file system events.

## Contributing

Contributions are welcome! If you have any ideas for improvements or new features, feel free to open an issue or submit a pull request.


