# file_organizer.py
import os
from pathlib import Path  # Correct capitalization of Path

def organize_files(directory):
    for file in os.listdir(directory):
        file_path = Path(directory) / file
        if file_path.is_file():
            ext = file_path.suffix[1:]  # Get extension without the dot
            target_dir = Path(directory) / ext
            target_dir.mkdir(exist_ok=True)  # Create folder if it doesn't exist
            file_path.rename(target_dir / file)  # Move file
            print(f"Moved {file} to {target_dir}")  # Display movement in terminal

# Replace "path_to_your_directory" with the actual path to the folder you want to organize
# Replace this path with the actual path to the folder you want to organize
organize_files("/home/isaiah2/automation.scripts/automation_scripts")
