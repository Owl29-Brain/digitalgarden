---
{"dg-publish":true,"permalink":"/3-d-experience-solidworks-questions/step-by-step-guide-to-performing-complete-clean-and-uninstall/","tags":["Troubleshooting","SOLIDWORKS"]}
---


The desktop version is already installed on the computer, please follow these steps to proceed with troubleshooting and uninstallation:

### Step 1: Download the Troubleshooter
1. Click on "Microsoft Program Install and Uninstall Troubleshooter" and select "Download Troubleshooter" from the link below:
   [Download Troubleshooter](https://support.microsoft.com/en-us/topic/fix-problems-that-block-programs-from-being-installed-or-removed-cca7d1b6-65a9-3d98-426b-e9f927e1eb4d)

2. Once downloaded, launch the troubleshooting pack.
   - When prompted with "Are you having a problem installing or uninstalling a program?", choose **Uninstalling**.

### Step 2: Select Programs to Uninstall
Choose to uninstall the following programs if they appear on the list:
   - **SOLIDWORKS** (any release found)
   - **SOLIDWORKS Visualize 20xx**
   - **Dassault Systèmes SOLIDWORKS 3DEXPERIENCE R20xxx**
   - **3DEXPERIENCE Launcher**
   - **CEF for SOLIDWORKS Applications**
   - **Dassault Systèmes Software VC10 Prerequisites x86-x64**
   - **Dassault Systèmes Software VC11 Prerequisites x86-x64**
   - **Microsoft Visual C++ 2015-2022 Redistributable (x64)**
   - **Microsoft Visual C++ 2015-2022 Redistributable (x86)**
   - **Microsoft Visual Studio Tools for Applications 2019**
   - **WPTx64**
   - **Visual Basic (VBA) 7.1**

### Step 3: Restart and Delete Specific Files
After uninstalling, restart the machine, then delete the following files if they exist:
   - `%programfiles%\Dassault Systemes\SOLIDWORKS 3DEXPERIENCE`
   - `%programfiles%\Common Files\SOLIDWORKS Shared`
   - `%programfiles(x86)%\Common Files\SOLIDWORKS Shared`
   - `%public%\Documents\Dassault Systemes`
   - `%public%\Documents\SOLIDWORKS`
   - `%programdata%\DassaultSystemes\3DEXPERIENCELauncher`
   - `%programdata%\SOLIDWORKS`
   - `%programdata%\SolidWorks HotFix`
   - `%appdata%\DassaultSystemes`
   - `%appdata%\SolidWorks`
   - `%localappdata%\TempSWBackupDirectory`
   - `%localappdata%\DassaultSystemes`
   - `%localappdata%\SolidWorks`
   - `%temp%\swcefcache`

   *(Note: ProgramData and AppData folders may be hidden. Enable "View hidden files" if needed, replacing `<User>` with the username or computer ID.)*

### Step 4: Delete Registry Keys
SOLIDWORKS retains registry keys to preserve settings during reinstallation. Delete the following registry keys to ensure a complete removal:
   1. Open **Control Panel -> Administrative Tools -> Registry Editor**.
   2. Navigate to each path below, and delete these registry keys:
      - `HKEY_CURRENT_USER\Software\Dassault Systemes\SolidWorks Shared`
      - `HKEY_CURRENT_USER\Software\Dassault Systemes\SolidWorksPDM`
      - `HKEY_CURRENT_USER\Software\SolidWorks`
      - `HKEY_LOCAL_MACHINE\SOFTWARE\Dassault Systemes\SolidWorksPDM`
      - `HKEY_LOCAL_MACHINE\SOFTWARE\Dassault Systemes\SwxConnectors`
      - `HKEY_LOCAL_MACHINE\SOFTWARE\Dassault Systemes\V6_Common`
      - `HKEY_LOCAL_MACHINE\SOFTWARE\SolidWorks`
      - `HKEY_LOCAL_MACHINE\SOFTWARE\Srac`
      - `HKEY_LOCAL_MACHINE\SOFTWARE\WOW6432Node\SolidWorks`

   **Note**: Modifying registry keys improperly may cause operating system issues. Proceed with caution during this step.