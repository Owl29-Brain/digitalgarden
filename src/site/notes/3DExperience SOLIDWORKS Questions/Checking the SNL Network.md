---
{"tags":["SOLIDWORKS"],"dg-publish":true,"permalink":"/3-d-experience-solidworks-questions/checking-the-snl-network/","dgPassFrontmatter":true}
---

#SOLIDNET 
# Step 1:Window Feature Enable
- From Control Panel > Programs > _**Turn Windows features on or off**_,
- Enable 3.5 Net framework and Telnet Client

![Pasted image 20240528163613.png](/img/user/3DExperience%20SOLIDWORKS%20Questions/Images/Pasted%20image%2020240528163613.png)
![Pasted image 20240528163640.png](/img/user/3DExperience%20SOLIDWORKS%20Questions/Images/Pasted%20image%2020240528163640.png)

- Press okay Go back to the control panel

# Step 2: Create the Inbound and Unbound connection 
_**SolidNetWork License Manager**_  
TCP port **25734** and **25735**

### Open Firewall and go to the Advance
![Pasted image 20240528163924.png](/img/user/3DExperience%20SOLIDWORKS%20Questions/Images/Pasted%20image%2020240528163924.png)
### Add New Rule in inbound
 
![Pasted image 20240528163950.png](/img/user/3DExperience%20SOLIDWORKS%20Questions/Images/Pasted%20image%2020240528163950.png)
### Select port and click next
![Pasted image 20240528164016.png](/img/user/3DExperience%20SOLIDWORKS%20Questions/Images/Pasted%20image%2020240528164016.png)
### Select TCP and add port values 
![Pasted image 20240528164040.png](/img/user/3DExperience%20SOLIDWORKS%20Questions/Images/Pasted%20image%2020240528164040.png)
### On next allows all the connection
 ![Pasted image 20240528164111.png](/img/user/3DExperience%20SOLIDWORKS%20Questions/Images/Pasted%20image%2020240528164111.png)
### Select all the option from below
![Pasted image 20240528164145.png](/img/user/3DExperience%20SOLIDWORKS%20Questions/Images/Pasted%20image%2020240528164145.png)
### Give a good name 
 ![Pasted image 20240528164201.png](/img/user/3DExperience%20SOLIDWORKS%20Questions/Images/Pasted%20image%2020240528164201.png)

### 3. ==Repeat steps 3-8 for Outbound and UDP Rules as well==
# Step 3: Telnet Check
- If you're here then 
- Write 
`telnet [IP] [Port number]`


# Step 4: Ping Test
- Perform the ping test from the command panel
`ping (Write down the IP)`

- If works then you're good to go
