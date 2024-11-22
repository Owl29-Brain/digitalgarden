---
{"dg-publish":true,"permalink":"/3-d-experience-solidworks-questions/how-to-remove-unwanted-files-in-solidworks-in-pack-and-go-and-missing-files/","dgPassFrontmatter":true}
---


- Make sure there is no external references in that file
- Remove all the views from the view pallets
- Derived/Mirrored Parts


**Missing Main Assembly:**

- **File Location:** Ensure the main assembly file and the drawing file are in the same folder or at least accessible to each other.
- **Drawing References:** Confirm that the drawing actually references the latest version of the main assembly.
- **Derived/Mirrored Assembly:** If the main assembly is derived or mirrored, pack and go the parent assembly instead.
- **Pack and Go "Include" Options:** In "Include Settings," make sure "Drawings/Configurations" is checked and the desired configuration of the main assembly is selected.