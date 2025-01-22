# Windows System Cleaner Automation

A simple PowerShell script and batch file setup to automate the cleanup of temporary files, prefetch data, recycle bin, and run Disk Cleanup on your Windows system. This tool is designed for quick execution via double-click or command line.

## Features

- Clears Windows and user temporary files.
- Deletes prefetch data to optimize performance.
- Empties the recycle bin.
- Runs Windows Disk Cleanup.

## How to Use

### 1. Clone the Repository
Clone the repository to your desired location:
```bash
git clone https://github.com/yourusername/windows-system-cleaner.git
```

### 2. Customize the Script
Open the clean.ps1 file and update the $BasePath variable if needed. Ensure it matches the path to the folder where the script is stored:
```bash
$BasePath = "C:\Path\To\Your\Folder"
```

### 3. Batch File Execution
The run_cleaner.bat file allows you to run the PowerShell script with a double-click. Ensure the path in the batch file matches the clean.ps1 file location:
```bash
powershell.exe -ExecutionPolicy Bypass -File "C:\Path\To\Your\Folder\clean.ps1"
```


### 4. Execute the Script
- Double-click the run_cleaner.bat file to start the cleanup process.
- Alternatively, run the PowerShell script directly:
```bash
.\clean.ps1
```


## Prerequisites
- Windows OS.
- Administrator privileges for running the script.
- PowerShell version 5.1 or later.

## Notes
- The script uses the -ErrorAction SilentlyContinue flag to suppress non-critical errors.
- Always test on a non-critical system or directory before using in production environments.

## Contributing
Feel free to fork this repository and contribute by submitting a pull request!

## License
This project is licensed under the MIT License.