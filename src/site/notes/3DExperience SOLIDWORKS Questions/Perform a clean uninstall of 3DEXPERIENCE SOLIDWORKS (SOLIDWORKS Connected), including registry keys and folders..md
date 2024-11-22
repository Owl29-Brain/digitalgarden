---
{"dg-publish":true,"permalink":"/3-d-experience-solidworks-questions/perform-a-clean-uninstall-of-3-dexperience-solidworks-solidworks-connected-including-registry-keys-and-folders/"}
---

#3DExperience #SOLIDWORKS #Troubleshooting
## Standard Uninstall

In _**most**_ cases, a standard uninstall is sufficient to resolve a problem that you have identified to _be_ an installation problem.

1. If you are working online, proceed to step 
2. **==If you are working offline, start SOLIDWORKS Connected, reconnect to your 3DEXPERIENCE platform, then close SOLIDWORKS Connected.==**
3.  Uninstall **Dassault Systemes SOLIDWORKS 3DEXPERIENCE R20XX** (Control Panel) 

## Intermediate Uninstall
In _**some**_ cases, a standard uninstall may not be sufficient, and you may need to perform a more comprehensive uninstall. 

1. Perform steps 1-3 of the standard uninstall procedure.  
2. In no particular order, uninstall:

1. Dassault Systemes Software VC10 Prerequisites x86-x64
2. Dassault Systemes Software VC11 Prerequisites x86-x64
3. Microsoft Visual C++ 2015-2022 Redistributable (x64)
4. Microsoft Visual C++ 2015-2022 Redistributable (x86)

## Advanced Uninstall

In **_extremely rare_** cases, an intermediate uninstall may not be sufficient, and you may need to perform an even more comprehensive uninstall.

Delete the following folders:

NOTE: Step 2 deletes some of these folders, some of these folders may not exist in your environment, and some of these folders may contain important user data like downloaded media, document templates, databases, and design library files.  
Always create a backup of the %public% and %programdata% folders before deletion.  

%programfiles% > Dassault Systemes> SOLIDWORKS 3DEXPERIENCE  
%programfiles% > Common Files > SOLIDWORKS Shared  
%programfiles(x86)% >Common Files > SOLIDWORKS Shared  
%public% > Documents > Dassault Systemes  
%public% > Documents > SOLIDWORKS  
%programdata% > DassaultSystemes > 3DEXPERIENCELauncher  
%programdata% > SOLIDWORKS  
%programdata% > SolidWorks HotFix  
%appdata% > DassaultSystemes  
%appdata% > SolidWorks  
%localappdata% > TempSWBackupDirectory  
%localappdata% > DassaultSystemes  
%localappdata% > SolidWorks  
%temp% > swcefcache_


4. Delete the following registry keys. Deleting the registry keys requires Windows administrative rights:

NOTE: Incorrectly editing the Windows Registry can severely damage your system. The SOLIDWORKS Technical Support team strongly recommends that you back up registry keys before making any changes or deleting.

HKEY_CURRENT_USER > Software > Dassault Systemes > SolidWorks Shared  
HKEY_CURRENT_USER > Software > Dassault Systemes > SolidWorksPDM  
HKEY_CURRENT_USER > Software > SolidWorks  
HKEY_LOCAL_MACHINE > SOFTWARE > Dassault Systemes > SolidWorksPDM  
HKEY_LOCAL_MACHINE > SOFTWARE > Dassault Systemes > SwxConnectors  
HKEY_LOCAL_MACHINE > SOFTWARE > Dassault Systemes > V6_Common  
HKEY_LOCAL_MACHINE > SOFTWARE > SolidWorks  
HKEY_LOCAL_MACHINE > SOFTWARE >Srac  
HKEY_LOCAL_MACHINE > SOFTWARE > WOW6432Node > SolidWorks_