#  Task 4: Setup and Use a Firewall (UFW on Kali Linux)

##  Objective
Configure and test basic firewall rules to allow or block traffic using **UFW (Uncomplicated Firewall)** on Linux.

---

##  Tools Used
- Kali Linux
- UFW (Uncomplicated Firewall)
- Terminal (bash)

---

##  Step-by-Step Guide

###  Check UFW Status  
Used the following command to check if UFW is active:

```bash
sudo ufw status
```


---

###  Enable UFW  
Enabled the firewall using:

```bash
sudo ufw enable
```


---

###  Block Inbound Traffic on Port 23 (Telnet)  
To block port 23 (commonly used by Telnet):

```bash
sudo ufw deny 23
```


---

###  Verify Rules  
To verify the current list of rules:

```bash
sudo ufw status numbered
```


---

###  Allow SSH (Port 22)  
To allow SSH access:

```bash
sudo ufw allow 22
```


---

###  Final Rule List  
Checked rules after allowing SSH:

```bash
sudo ufw status numbered
```


---

###  Remove the Test Rule (Port 23 Block)  
To clean up the rule used for testing:

```bash
sudo ufw delete deny 23
```

###  Disable UFW Firewall 
To disable UFW firewall:

```bash
sudo ufw disable
```

## Attachments

- `Status.png` – Shows UFW Disable status
- `Enable_UFW.png` – Show UFW enable
- `Telnet_Rule.png` – Shows Telnet (Port 23) rule added
- `Rule_Verification.png` – Final rule verification with SSH and Telnet
- `Remove_Rules.png` – Shows Remove Rules
- `Disable_UFW.png` – Show UFW disabled
