---
{"dg-publish":true,"permalink":"/3-d-experience-solidworks-questions/how-to-deal-with-solidworks-resource-running-low/"}
---

https://blogs.solidworks.com/tech/2018/10/how-to-deal-with-solidworks-resource-running-low.html

# **SOLIDWORKS Resource Running Low**

![SOLIDWORKS Resource Monitor](https://blog-assets.solidworks.com/uploads/sites/4/SOLIDWORKS-Resource-Monitor.png)

Some SOLIDWORKS users tend to encounter this issue. Factor such as limited RAM space and many running programs at one time can be considered as the major caused.

For resolution, you may refer the to 2 options below.

1. Virtual Memory Setting
2. Registry modification

The cause of the Resource Monitor warning message is due to the GDI Objects limit of your Window OS. GDI object limit for a single process to be 10,000 by default. However, it has the maximum allowed up to 16384. By increasing the limit, each application will be in a comfort zone.

We will always suggest user to upgade the custom size in the Virtual Memory first instead of modifying the registry settings. If this resolved, no modification of the registry settings is required.

In the event, that this doesnt resolve, then you will need to modify the registry settings.

There are no guarantee that problems resulting from modifications to the registry can be solved at one time. There are risk in modifying the window registry which eventually cause Window operating system error. **Reinstall of your operating system is required in this case.**

## **Method 1: The Virtual Memory Settings**

1. Go to Control Panel> System > Advanced System Settings

![Advanced system setting](https://blog-assets.solidworks.com/uploads/sites/4/Advanced-system-setting-615x450.png)

2. Advanced (Tab) > Settings

![](https://blog-assets.solidworks.com/uploads/sites/4/Setting.png)

3. Advanced > Change

![Advanced > Change](https://blog-assets.solidworks.com/uploads/sites/4/Advanced-Changed.png)

4. Uncheck “Automatically manage paging file size for all drives”.Choose the Driver which you would prefer to utilise the virtual memory.

5. Under Custom size, enter the value double the size of the amount of physical RAM installed in your PC. (If you have 16GB, type in 32000MB)

![](https://blog-assets.solidworks.com/uploads/sites/4/custom-size-227x300.png)

6. Enter the Initial size value of 2 times the amount of physical RAM installed in your system (eg. If you have 16GB, type in 32000MB.)

7. Click on ‘Set’.

8. Restart your workstation.

**Monitoring**

You may monitor this through the Task Manager. This solution will involve editing the Windows Registry.

1. Open Task Manager (right click on start bar > Task Manager OR through CTRL+ALT+DEL)
    - ![](https://blog-assets.solidworks.com/uploads/sites/4/Task-Manager-300x196.png)
2. Click on ‘Details’ Tab
    - ![](https://blog-assets.solidworks.com/uploads/sites/4/Details-Tab-615x174.png)
3. Right-click on one of the columns and click  ‘Select Columns’
    - ![](https://blog-assets.solidworks.com/uploads/sites/4/Select-Column-615x169.png)
4. Tick the GDI objects
    - ![](https://blog-assets.solidworks.com/uploads/sites/4/GDI-283x300.png)
    - ![](https://blog-assets.solidworks.com/uploads/sites/4/GDI-Task-manager-615x279.png)

**Method 2: The Registry Settings**

1. Open **Regedit** (via Run > type ‘**regedit**’)
2. Locate to the key: HKEY_LOCAL_MACHINE> SOFTWARE> Microsoft> Windows NT> CurrentVersion> Windows>  GDIProcessHandleQuota
3. Right click on the ‘**GDIProcessHandleQuota**’ and click ‘**Modify**’.
4. Change the registry key to the maximum process limit **16,384**; set the **BASE** to **DECIMAL**.
    - ![](https://blog-assets.solidworks.com/uploads/sites/4/Registry-300x153.png)

**Take note that altering Window registry can cause Window OS malfunction.

Alternatively, if you just wish to dismiss the message, you always have the option to do so from the Window Toolbar Notification area.

![](https://blog-assets.solidworks.com/uploads/sites/4/dismiss-graphics-noti.png)