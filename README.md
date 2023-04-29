# File Integrity Monitoring (FIM) Project

This project is a basic implementation of a File Integrity Monitoring (FIM) tool using PowerShell. The script monitors a set of files for changes and notifies the user if a file has been created, modified, or deleted.

## How it works

The script has two main functionalities:
- Collecting a baseline hash for each file in the target folder and storing it in a text file named "baseline.txt".
- Continuously monitoring the target folder for changes by calculating the hash of each file and comparing it with the hash stored in "baseline.txt".

If a new file has been created, the script will notify the user by printing the file name in green. If an existing file has been modified, the script will print the file name in yellow. If a file has been deleted, the script will print the file name in dark red with a gray background.

## How to use

To use this script, follow these steps:
1. Clone the repository to your local machine.
2. Open PowerShell and navigate to the directory where the script is located.
3. Run the script using the command `.\FIM.ps1`.
4. Choose between collecting a new baseline or monitoring files with the saved baseline.

## Next steps

- Add the ability to log the notifications to a file or send them via email.
- Implement support for monitoring subfolders.
- Implement support for monitoring network shares.
- Add the ability to exclude files or folders from monitoring.
- Improve error handling and reporting.
