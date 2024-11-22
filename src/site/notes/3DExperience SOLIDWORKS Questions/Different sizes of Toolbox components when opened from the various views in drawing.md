---
{"dg-publish":true,"permalink":"/3-d-experience-solidworks-questions/different-sizes-of-toolbox-components-when-opened-from-the-various-views-in-drawing/","tags":["Service_Request"]}
---


# Message 1
The customer is experiencing an issue with SOLIDWORKS when attempting to open files from the Product Data Management (PDM) system, as demonstrated in a captured video. 

Upon opening a drawing file in SOLIDWORKS, it was observed that the size of the toolbox components changes depending on which view is used to open the file. 

After investigating, it was determined that rolling back and saving the files from the PDM system in the latest version resolved the issue in certain cases, but the fix did not apply to all files.

Let me know if you'd like to add or modify anything further.
# Message 2
- Check the issue using the PDM admin login to determine if the same behavior occurs.
- Open the assembly first and verify if the toolbox components inserted in the assembly display the correct size.
- Disable the toolbox option 'Make this folder the default search location for Toolbox components' and confirm if the toolbox components display the correct size.
# Message 3
Yes with Admin login have the same effect. Yes, if the assembly opens the first sizes are showing correctly. If disabling the Toolbox and setting location to default is having a worse effect actually, it makes all sizes too big.
# Message 4
It was noted that disabling the "Make this folder the default search location for Toolbox components" option did not resolve the issue. To gain more clarity on how the Toolbox is integrated, the following details were requested:

- Clarification on whether the Toolbox is installed locally or integrated with the PDM Vault.

Additionally, to assist in further investigation, the following actions were requested:

- Provide a screenshot of the Toolbox settings (Open Administration Tool, go to SOLIDWORKS > Toolbox).
- Open the same drawing shown in the video, disable the PDM Add-in, and then open the assembly from the view to check if the issue persists.
- Test the workflow on a different machine to determine if the problem occurs there.
- Confirm if the issue is happening with a specific drawing or all drawings within the PDM Vault.
- Check the behavior outside the PDM environment and confirm whether the issue is reproducible.

Awaiting the response to continue troubleshooting.
# Message 5
Dhruval provided additional information regarding the ongoing SOLIDWORKS PDM issue, along with three videos demonstrating the issue when opening files from PDM (the sequence may vary). In one of the videos, selecting 'open' temporarily resolved the issue; however, upon reopening, the issue persisted.

Details from the investigation:

1. A screenshot of the Toolbox settings has been provided for review.
2. Disabling the PDM Add-in did not resolve the issue, and the component sizes still differed when opening from different views.
3. On other machines, the issue could not be reproduced.
4. The issue occurs in specific drawing files but not universally.
5. Outside the PDM environment, the issue does not occur.

The next steps for further investigation and resolution can be determined based on this additional information.
# Message 6
It was noted that the Toolbox appears to be integrated within the PDM Vault. The videos will be reviewed as part of the ongoing analysis, and an update will be provided once the review is complete.

Let me know if any further details are needed!
# Message 7
Dhruval emphasized the urgency of the issue, as the drawing in question has already been released, and other tasks are pending due to this specific file. A prompt solution would be greatly appreciated.

Thank you for the understanding, and please expedite the resolution process.
# Message 8
After reviewing the video, it was determined that the issue is occurring on a single client machine. A remote session has been suggested to investigate and troubleshoot the problem more closely. 

A meeting has been scheduled for tomorrow at 11 AM. The details are as follows:

- **Meeting URL:** [Join the Meeting](https://3ds.zoom.us/j/81195726068?pwd=oXv07bbWwGMaKK3haHAuFFCP7L4wj8.1)  
- **Meeting ID:** 811 9572 6068  
- **Passcode:** 307062  

Participants are requested to join the meeting to address the issue.
# Message 9
It was noted that the meeting is scheduled for 11 AM today. The customer has expressed interest in joining the session. 

To facilitate this, Dhruval can either take remote access from the customer or share the meeting link so the customer can join the session directly.
# Message 10
It has been decided that the customer does not need to attend the meeting at this time, as the issue requires troubleshooting. However, if additional details or assistance are needed during the session, Dhruval may request the customer's participation.
# Message 11
Following the discussion, the investigation into the issue with the drawing view displaying the incorrect toolbox component revealed that the problem occurs even with Admin login and across multiple client machines. It was found that opening the assembly file first and then the drawing file prevents the issue, serving as a temporary workaround.

To proceed, the following actions are requested:

1. Recreate the drawing view and check if the problem persists.
2. Provide the customer database and the archives from the assembly/toolbox folder to facilitate replication of the issue.

Dhruval is available for any further questions or clarifications needed.
# Message 12
Dhruval apologized for the delay and has attached the requested files for review. Additionally, it was noted that the customer is not willing to share the design files; however, all other necessary files have been provided.

The review of the attached files will proceed to further investigate the issue.
# Message 13
The request has been made for the customer archives to investigate and replicate the behavior on our end. This step is crucial to determine the root cause of the issue, especially since it is observed across multiple logins and client machines.

If the customer has security concerns regarding sharing partial archives, they can initiate the Non-Disclosure Agreement (NDA) process. Otherwise, providing a reproducible workflow would be helpful for replicating the issue on Dhruval's machine.

In light of the available workaround, the severity rating has been lowered to "High" to align with its urgency level.
# Message 14
Dhruval has already attached the archives and is uncertain about what additional files are required for testing. It was clarified that an assembly file may not be necessary, as the issue has been observed across various files.

Dhruval is open to clarification if there has been any misunderstanding regarding the requirements.
# Message 15
It was clarified that the reference to "partial archives" specifically pertains to the assembly and drawing files, along with their child references, necessary to replicate the issue on Dhruval's end. The zip file provided earlier included toolbox files and a PDM database backup but did not contain the required archives.

To assist in retrieving the selected assembly and its references, Dhruval can refer to the following Knowledge Base (KB) article:

- **Article ID:** QA00000109503  
- **Abstract:** Is there a tool to copy only selected file archives (partial copy) from a SOLIDWORKS® PDM file vault archive for testing purposes?  
- **Link:** [KB Article](https://support.3ds.com/knowledge-base/?q=docid:QA00000109503)  

This guidance will help in obtaining the necessary files for further investigation.
# Message 16
It was reported that an attempt was made to create a partial copy using the provided tools, but the process was unsuccessful. The following tools were utilized:

1. **Collect Support Information**
2. **Archive Copy Tool**

Both attempts failed because the option to copy the archive was not available in the Archive Copy Tool, leading to difficulties in obtaining the necessary files for testing. Further assistance may be required to resolve this issue.
# Message 17
It was noted that the **Collect Support Information** tool cannot gather archives due to a reported bug. The previously referenced QA article should assist in retrieving the necessary archives.

To facilitate further troubleshooting, a request was made for a screen recording of the steps being taken to collect the archives using the tool. This will help identify any issues in the process.
# Message 18
Dhruval has attached a screen recording demonstrating the steps taken to collect archives using the **Get Archive Tool** mentioned in the QA article. It was noted that the option to copy the archive does not appear after adding the file archives.

This recording will help diagnose the issue further.
# Message 19
As discussed during the meeting, it is requested that the archives of the problematic drawings, assemblies, and their child references be shared, along with the toolbox data folder. These files will be crucial for further investigation into the issue.
# Message 20
Dhruval is familiar with the process on the server but is encountering difficulties using the **Get Archives Tool** on a client PC without access to an Archive Server or Database Server. Guidance is requested on how to effectively utilize this tool in such an environment.

Additionally, it was noted that the customer is unwilling to share the archive files, despite explanations regarding the NDA terms, due to their company policy. They have proposed sharing the archive file with suppressed components instead, indicating they would suppress the components first before sharing the archives.
# Message 21
It was inquired whether there are any issues being encountered with the **Get Archives Tool** when running it from a client. If using a non-archive server client, it is important to ensure that a UNC (//) path is used and that the client machine has access to the vault archives.

Additionally, it was noted that if the files are suppressed, they will appear hidden in the drawings, which may hinder the ability to replicate the behavior for further investigation on Dhruval's end.
# Message 22
Dhruval has spoken with the customer, who has confirmed they are not willing to share any files due to company policy. The customer is requesting an alternative method to resolve the issue without sharing the files.
# Message 23
Requested to know if the issue can be reproduced in the customer vault using the sample fileset. If it can be reproduced, Dhruval asks for an outline of the steps followed to replicate the behavior on his end. In the meantime, he will check internally and keep the customer updated on how to proceed with further analysis and investigation.
# Message 24
Set message from Satish outlining the steps and observations regarding the issue with the drawing file and toolbox components in the PDM.

1. **Opening Drawing File from PDM:** When the drawing file is opened directly from the PDM, it may or may not contain toolbox components in the views.
    
2. **Issue with View Size:** Clicking on the view that has the issue will show that the sizes are bigger. It is noted that the issue is related to the configuration on the drawing.
    
3. **Errors While Closing Assembly:** While closing the assembly, there are instances where errors appear, and components may change automatically. Before closing, SOLIDWORKS sometimes displays 2-3 error messages, but this does not always resolve the issue.
    
4. **Opening from Non-Issue View:** If the file is opened from a view that does not have issues, the sizes remain intact without any problems.
    
5. **Workaround:** The workaround is to open the assembly first from the PDM and then the drawing file. This method does not lead to the issue. There is no visible problem if the part is not saved in the PDM.
    
6. **Issue After Saving:** However, reopening the file after saving still results in the same issue.
    

# Resolution
On the customer site issue has been resolved by replacing toolbox file with the available on the desktop
Then that file was checked in 
Afterwards, file was made available for everyone
Name of the file and location was the same so there were no need to add location in the other PCs