---
{"dg-publish":true,"permalink":"/3-d-experience-solidworks-questions/new-installation-of-solidworks-crashing-at-splash-screen/"}
---

#SOLIDWORKS #Troubleshooting 
## First Solution

The support team at Hawk Ridge Systems has found success in replacing the libcef.dll file with file version 100.0.14.0 to resolve the issue. You can see which version the dll file is in by right-clicking on the file in File Explorer > Properties.

1. Download the libcef.dll file here: [download link](https://d1p8f5d0ap7dbx.cloudfront.net/Support%20Tools/libcef.zip?Expires=1730390414&Signature=HL8ehHFIwcU1ZpKHVujyCKY6nShN31AKV3MbP6CW-xZWx6B~qA1eu4KhqZTeW6U63J34piXTnaOttUYdMn0ItoTPKxCReUzK~I32go1~-K~oYPgWOZBGF4M5Z2EbEKDnXBd06XKWnQUcdTQW7fAiqGSJ84pG2gjwiSJwuXsegIc7J2TLgaQT1KFAvwgS0rS6mBY8KJGv5ojQQcSHo7QIp7OajbbtGsb7V~1imXHaJJYFngIvYfpdX8yV1Ypemm7OJRWPc88xp2JzYWFzWXkaPUdzrpreuhdgI-JEWzyiqhl7iMB7z3lIeLItYGQ2Pi77xwISlRqvsq3KFi9R8bO~6g__&Key-Pair-Id=APKAJPRFTZHLVUVJGMJQ)
2. Browse to C:\Program Files\Common Files\SOLIDWORKS Shared\swcef\
3. Replace the libcef.dll in the folder with the one downloaded from Step 1.

## Second Solution

In this solution, we will let SOLIDWORKS reinstall the components it needs by renaming a folder that SOLIDWORKS will recreate with a repair.

1. Browse to C:\Program Files\Common Files\SOLIDWORKS Shared\
2. Rename the "swcef" folder to "swcef-old"
3. Repair SOLIDWORK