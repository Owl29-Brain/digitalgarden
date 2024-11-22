---
{"dg-publish":true,"permalink":"/3-d-experience-solidworks-questions/design-tree-not-visible-and-system-crashing/"}
---

#Service_Request #SOLIDWORKS #Troubleshooting 
# Response 1
An issue has been identified when opening assemblies in SOLIDWORKS. The problem affects various assemblies and does not appear to be file-specific. Occasionally, after the assembly components load, the progress bar fails to display, the design tree becomes invisible, and SOLIDWORKS becomes unresponsive. This error occurs randomly, and it has not been possible to reproduce the issue consistently or identify the exact cause.

# Response 2
1. The Rx does not include the system information file. Please provide the system information file. Additionally, verify whether the system is SOLIDWORKS certified.
2. Capture a video of the issue when it occurs.
3. Specify which assembly was affected. Is it a large or complex assembly?
4. Share the assembly file. Indicate the number of components in the assembly.
5. Are the files stored on a network?
6. When was the issue first observed? Were there any recent hardware or software changes?
7. Is the issue only noticeable with assembly files? What is the behavior with part files and other assemblies?
8. Confirm whether the issue occurred while working on SNL. Was the license borrowed at the time of the issue?

# Response 3
1. Tomorrow, the customer will be asked to create a new Rx. However, the hardware has been checked and is confirmed to meet the SOLIDWORKS Certified Basic Specification, featuring an NVIDIA RTX A2000 8GB.
2. Capturing a video of the issue is not possible due to its random occurrence. If the explanation provided does not fully describe the issue, clarification will be sought.
3. The issue has been reported with various files, affecting both assemblies and parts, regardless of their size.
4. Sharing the files is not feasible.
5. The customer uses SOLIDWORKS PDM.
6. The issue arose after upgrading to SOLIDWORKS 2024 on all systems.
7. The behavior is observed in both assembly and part files.
8. The customer is not borrowing the license.

# Response 4
1. Please provide the complete Rx capture along with a video and system information file.
2. Test the issue outside the PDM environment by copying the files to a local machine and checking if the behavior can be reproduced.
3. For testing purposes, borrow a license and verify if the behavior is reproducible.
4. Indicate how many machines exhibit the same issue.
5. Test the behavior in OpenGL mode and report the results.
6. Identify the version from which SOLIDWORKS was upgraded to 2024.
7. After the upgrade, were the files saved in the latest version? For testing, open the file in SOLIDWORKS 2024, save it, and observe if the issue persists when the same file is reopened.
8. Since the issue is random, provide a sample file that demonstrates the problem on the customer’s machine, along with the Rx, for further testing.

# Response 5
The issue appears to be system-specific. According to the information provided, the problem arises when SOLIDWORKS runs in the background and causes the system to crash or freeze. For instance, if Chrome is being used while SOLIDWORKS is running in the background, it results in a system crash or freeze. However, if SOLIDWORKS is not running, the issue does not occur.

It seems to be related to the system's specifications, but there is no current connection with the user. Once contact is reestablished, the Rx and, if possible, a video will be shared for further analysis.

# Response 6
1. Efforts to capture the issue have been inconsistent due to its random nature. The issue did not occur during some attempts.
2. The system continues to crash even after the files were tested outside of PDM.
3. Testing with a borrowed license has been requested, but due to the customer's schedule, this could not be performed live. Further details will be provided once testing is completed. The issue began after the latest update.
4. The issue is observed on only one machine.
5. The customer is currently unavailable, so only an Rx file has been created.
6. The customer was using SOLIDWORKS 2024 SP2 before the latest update.
7. All files are in the latest version, and they are working with the updated file formats.
8. The customer is not willing to share files, and the issue affects all file types, including parts, assemblies, and drawings.

# Response 7
1. From the logs, a crashing event of SOLIDWORKS was identified on August 12th. The faulting application was `sldworks.exe`, version 32.3.1.2, with the faulting module being `ntdll.dll`, version 10.0.22621.3733.
2. Additionally, a hanging event of SOLIDWORKS was noted on August 16th.
3. Multiple application crashes have been observed, with `ntdll.dll` identified as the faulting module for these events. The module version is 10.0.22621.3733, and the timestamp is 0x67ca8829. It is recommended to connect with the IT team to repair the faulty module and retest the issue.
4. If the issue persists after repairing `ntdll.dll`, consider repairing the operating system and testing the behavior again.

Additionally, capture an image or video, along with the Rx, when the issue occurs again. Identifying the exact cause may be challenging without knowing the specific workflow to reproduce the issue. The customer should be advised to observe and document the workflow carefully before the issue arises and re-verify it.


# Response 8
The customer has reported that the issue is no longer occurring, and it is believed to be resolved. Thank you for your prompt support. The service request can now be closed.
