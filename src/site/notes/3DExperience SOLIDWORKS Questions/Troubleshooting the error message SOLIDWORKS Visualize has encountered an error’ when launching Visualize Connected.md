---
{"dg-publish":true,"permalink":"/3-d-experience-solidworks-questions/troubleshooting-the-error-message-solidworks-visualize-has-encountered-an-error-when-launching-visualize-connected/","tags":["Troubleshooting","Visualize"]}
---

Error Occurs in following format, while launching SOLIDWORKS Visualize![](https://blog-assets.solidworks.com/uploads/sites/4/1-153-615x277.png)

**Possible reasons that could cause this error:**

A. **If there is corruption in the SOLIDWORKS® Visualize settings.** You can initialize the basic troubleshooting by doing:

First, kill SWVisualize.Queue.Server.exe process from task manager and rename below folders

- - 1. _%USERPROFILE%\Documents\SOLIDWORKS Visualize Content_
        2. _%LOCALAPPDATA%\Dassault_Systèmes\SLDWORKSVisualize.exe…._
        3. _%LOCALAPPDATA%\SOLIDWORKS\SOLIDWORKS Visualize <version>_
        4. _%PROGRAMDATA%\SOLIDWORKS\SOLIDWORKS Visualize <version>_

B. **User may have two different graphics adapters (Discrete and Integrated)** in a machine, and Visualize might be using integrated display adapter. In this case, dedicate Visualize to run on GPU (NVIDIA or AMD) using following steps:

- - 1. Go to Start menu and type **Settings**
        2. Select **System** and click on **Graphics settings**
        3. Under **Choose an app to set preference**, browse **SLDWORKSVisualize.exe** from the installation location of Visualize Connected **[**_**C:\Program Files\Dassault Systemes\SOLIDWORKS 3DEXPERIENCE\Visualize]**_
        4. Click on **Options** and set the graphics preference to GPU under **High Performance**
        5. Save the settings

During diagnosis, it was observed that above suggestions followed by update of latest graphic drivers, clean reinstall of SOLIDWORKS Visualize Connected did not worked. However, customer disabled the integrated (Intel) graphics card and this fixed the problem.

**Disclaimer:** Disabling a graphics card is not recommended. If the problem is discrete graphics card related, then user needs to contact their IT Admin or Hardware Vendor and make sure that Visualize also utilizes GPU.