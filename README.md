# Vulnhub-Vulnix


![image](https://github.com/user-attachments/assets/828bf411-91c9-4481-8582-d1b188937fec)

## 📌 Project Objective

The objective of this challenge was to perform a full penetration test on the Vulnix vulnerable machine hosted on VulnHub. This involved identifying open ports and services, exploiting misconfigured network services, and escalating privileges to gain root access. The exercise aimed to simulate real-world enumeration and exploitation techniques on a Linux-based target, enhancing practical skills in reconnaissance, service enumeration, privilege escalation, and post-exploitation.

## 🧠 Skills Learned

- 🔹 **Network Scanning & Enumeration** – Used tools like Nmap to identify open ports, services, and potential entry points.
- 🔹 **Service Enumeration** – Analyzed services like NFS, SSH, and RPC for misconfigurations and vulnerabilities.
- 🔹 **NFS Exploitation** – Learned how to mount and exploit misconfigured NFS shares to access sensitive information.
- 🔹 **Privilege Escalation** – Practiced escalating user privileges to root through weak configurations and known techniques.
- 🔹 **Linux System Enumeration** – Gained experience in identifying system information, user privileges, and exploitable paths.
- 🔹 **Manual Exploitation** – Strengthened hands-on exploitation skills without relying on automated tools.
- 🔹 **CTF Methodology** – Reinforced a structured approach to Capture The Flag (CTF) machines, from reconnaissance to root.


## 🛠️ Tools Used

- 🔍 **Nmap** – Scanned for open ports and performed service/version detection.
- 📡 **RPCinfo & Showmount** – Enumerated RPC services and mounted NFS shares to discover accessible data.
- 🧰 **Metasploit Framework** – Used to automate exploitation and post-exploitation tasks.
- 🐚 **Kali Linux Terminal** – Primary environment for conducting reconnaissance, exploitation, and privilege escalation.
- 🛠️ **Netcat** – Used for setting up reverse shells and testing open ports.
- 🔒 **SSH** – Secured shell access to the target once credentials were acquired.
- - 🐍 **Hydra** – Bruteforced login credentials on services like SSH.
- ⚙️ **Linux Privilege Escalation Scripts** – Identified local misconfigurations and escalation opportunities.


## Steps
## 🧭 Step-by-Step Attack Summary

- **Network Scanning**  
   Used `nmap` to identify open ports and running services, revealing NFS and RPC services.

   ![image](https://github.com/user-attachments/assets/c9879b75-23f2-4b22-abdc-09ae0729d2ef)


- **Service Enumeration**  
   Leveraged `showmount` and `rpcinfo` to enumerate accessible NFS shares and RPC endpoints.

 

- **SMTP Exploitation via Metasploit**  
   Leveraged Metasploit to exploit a vulnerable SMTP service, allowing enumeration of users or potential remote code execution (depending on exploit module used).
     ![image](https://github.com/user-attachments/assets/4243c9a6-815b-4659-8d79-bfdd39f69c48)

- **Finger Exploitation via Metasploit**  
   Leveraged Metasploit modules targeting the vulnerable Finger service to extract usernames or other system details.

   ![image](https://github.com/user-attachments/assets/03714515-843b-48de-82d5-15861ba17d47)

   ![image](https://github.com/user-attachments/assets/92a9c8fc-f331-4daa-8350-f06cca0a7d6c)

- **Finger Service Enumeration (Auxiliary Module) Option 10 for Exploit**  


   ![image](https://github.com/user-attachments/assets/0121fcaa-7d86-4844-8291-ddadd8bd9e0f)

- **Brute-Force Attack via Hydra**  
   Executed a brute-force attack on SSH using `Hydra`, leveraging discovered usernames.

   ![image](https://github.com/user-attachments/assets/6fc0bbe2-0b37-4de3-9bc6-a9d5ed4d3997)

- **Initial Shell Access via SSH**  
   Logged into the system via SSH with valid credentials obtained through brute-forcing.

   ![image](https://github.com/user-attachments/assets/925495ca-8884-45b6-9899-1267bf0ff2e4)

   ![image](https://github.com/user-attachments/assets/3bb046fb-803b-40e3-856b-320d3fb3687d)


   ![image](https://github.com/user-attachments/assets/3302ce58-4ea8-4c14-a1d9-36c5c0576717)

- **Root Access & Flag Retrieval**  
   Gained root access and captured the final flag, completing the challenge.

   ![image](https://github.com/user-attachments/assets/a8d3b4c4-db9c-4821-b21e-ba7830475ce8)










     




