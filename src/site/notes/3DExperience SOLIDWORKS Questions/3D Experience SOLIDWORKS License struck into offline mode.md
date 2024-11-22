---
{"dg-publish":true,"permalink":"/3-d-experience-solidworks-questions/3-d-experience-solidworks-license-struck-into-offline-mode/"}
---

#Service_Request #3DExperience #SOLIDWORKS 
# Initial Issue
While reinstalling SOLIDWORKS 3DEXPERIENCE due to technical reasons, I discovered that the system was offline (After uninstalling). After completing the uninstallation and attempting to relaunch SOLIDWORKS, I encountered an error message stating: "Could not obtain the required license for SOLIDWORKS Connected. Check your roles assignments and try again."

![2024-03-14 17_37_19-948 512 471 - AnyDesk.jpg](/img/user/3DExperience%20SOLIDWORKS%20Questions/Images/2024-03-14%2017_37_19-948%20512%20471%20-%20AnyDesk.jpg)


# Response from DS: Initial steps 
1. Close SOLIDWORKS. 
2. Open Browser (Firefox\Chrome\Edge) > Clear all browser data.
3. Go to 'Compass > Preferences (Left side gear icon) > Roles and Apps display > Select Current Platform.
4. Go to 'Platform Management -> Members -> Configure Members Option > Turn On: Automatically ungrant expired roles from members or groups
5. Go to 'Platform Management > Members > Members Control Center > Invite & Grant Roles,' ungrant the current SOLIDWORKS Roles, and grant the roles again.
6. Clear browser data and Login to Platform.
7. Go to 'Compass > 3DSpace
8. Create new collaborative space (If required).
9. Select a collaborative space.
10. Go to 'Compass > Collaboration and Approvals -> Profile -> Refresh My License
11. In Compass, click on SOLIDWORKS to launch SOLIDWORKS.

### If the issue persists

1. Fiddler Traces with video recording. Article ID: QA00000038204 Abstract: Using the FiddlerCap utility to collect network traces Link: https://support.3ds.com/knowledge-base/?q=docid:QA00000038204
2. Logs' folder from following location. C:\ProgramData\DassaultSystemes\3DEXPERIENCELauncher\ (Program data folder might be hidden please turn on Hidden folder visibility)
3. ‘SWXDesktopLauncher’ and ‘SWXDesktopHelper’ folders from following location. C:\Users\<You>\AppData\Roaming\DassaultSystemes\

# Issue in following steps
steps 1 to 4, the license remains stuck on offline status. because of that I'm unable to proceed with the troubleshooting steps.
New space as advised, but unfortunately, this did not resolve the issue either.
# Further Steps: Checking registry file location and editing 
Try below

Check to see if the registry key exists and if it is set to Offline.
1. The registry key is found here [\HKEY_CURRENT_USER\SOFTWARE\ Dassault Systemes\SolidWorks Shared\Servers\3DEXPERIENCE].
2. "Enable Offline Mode"=dword:00000001. Edit this key to "Enable Offline Mode"=dword:00000000" 2. Reboot and start SOLIDWORKS Connected. 
3. Switch back to Online, if successful the software should reconnect to the cloud in MySession. 
4. If it still fails and the Registry key is correct as "Enable Offline Mode"=dword:00000000" 
5. Check to see if the License files exist in the location above. 
6. If they are present , move them to a new folder, Reboot and start SOLIDWORKS Connected.

# Issue in following steps
Registry path you provided does not exist: [\HKEY_CURRENT_USER\SOFTWARE\Dassault Systemes\SolidWorks Shared\Servers\3DEXPERIENCE].


# Furthered steps: Creating Registry file manually 
Caution: Incorrectly editing the registry can severely damage your operating system. The SOLIDWORKS Technical Support team strongly suggests that you back up the registry data before making any changes to the registry. 

The new reg key should be Hexadecimal not Decima 
1. Go to the registry editor (Note reg names must be exact 
2. Browse to the reg key [\HKEY_CURRENT_USER\SOFTWARE\Dassault Systemes\SolidWorks Shared\Servers\3DEXPERIENCE]. 
3. Create a new 32 bit DWORD key. 4
4. Value = OfflineFromConnected 
5. Value data = 0 6. Close registry editor 
6. Reboot PC and start SOLIDWORKS Connected.

# Final Step
Replacing the key from following location
C:\ProgramData\DassaultSystemes\Licenses

Copy and place the license on the desktop and try after that try again launching from the shortcut.

In this case this works!