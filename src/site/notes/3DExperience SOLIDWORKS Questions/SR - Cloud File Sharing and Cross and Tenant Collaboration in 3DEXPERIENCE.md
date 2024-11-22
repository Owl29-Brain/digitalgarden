---
{"SR":"SR01267340-01","tags":["Service_Request","3DExperience"],"dg-publish":true,"permalink":"/3-d-experience-solidworks-questions/sr-cloud-file-sharing-and-cross-and-tenant-collaboration-in-3-dexperience/","dgPassFrontmatter":true}
---

1. **Sharing files on the cloud:**
    
    - **Question:** Is it possible to "share" files directly on the cloud, even though external users have no access to the cloud? Put simply, can they upload the file to their own tenant?
        
    - **Answer:**
        
        - No, in order to save files to the tenant on the cloud, users must have access to the tenant on the cloud.
        - You can invite any user with external user rights.
        - The reverse is possible: you can share files from 3DDrive to any external user who has a 3DPassport account, even if they have no access to your tenant.

---

2. **Collaboration between two 3D Experience licenses (India and USA):**
    
    - **Question:** They have two 3D Experience licenses—one in India and one in the USA. If they don't have the same tenant, how can they work in collaboration?
        
    - **Answer:**
        
        - I understand that you have two different tenants, and you want users from Tenant A to collaborate with users from Tenant B.
        - This functionality is possible and is called "cross-company collaboration." Only an admin can set this up for its members.
        
        **Steps:**
        
        - **Tenant A:**
            - Go to **Configure Members** option.
            - Enable: "Allow administrators to grant roles without assigning automatically the associated license."
            - For the existing user (e.g., abc@xyz.com) of your choice, disable "Restrict usage to this platform" for the 3DSwymwe role.
        - **Tenant B:**
            - abc@xyz.com is not available on this tenant.
            - Go to **Configure Members** option.
            - Enable: "Allow administrators to grant roles without assigning automatically the associated license."
            - Invite abc@xyz.com with the "Assign License" option disabled.
        
        **Conclusion:**
        
        - abc@xyz.com was already present on Tenant A with roles as well as licenses (can log in to Tenant A).
        - We invited abc@xyz.com to Tenant B without any licenses, only with a role.
        - Result: abc@xyz.com can log in to Tenant B using licenses from Tenant A and roles from Tenant B.
        
        **Important:**
        
        - These steps should be followed with utmost care. If licenses are mistakenly assigned on Tenant B, they will be locked for 30 days.
        - If you have any doubts, please open a new SR so a dedicated cross-company functionality expert can assist you.