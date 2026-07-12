# Linux Services, SSH, Firewalls & Compression

•	- Install and configure Apache, SSH server, and firewall (UFW).
•	- Test web service accessibility over LAN.
•	- Use nmap to detect open services and ports.
•	- Use SSH and SCP for remote access and file transfer.
•	- Create and manage users and understand privilege separation.
•	- Compress and decompress files using tar and bzip2.
•	- Troubleshoot VirtualBox VM network conflicts (MAC/IP clash).
Lab Activities
•	- Install Apache using `sudo apt install apache2` and test `http://127.0.0.1`.   
•	- Install SSH server and Nmap: `sudo apt install openssh-server nmap`.  
•	- Determine IP using `ip a` and visit peer web page in browser.    
•	- Edit index.html using nano/gedit and share unique changes with partner.
•	- Scan each other's ports using `nmap [IP]` and note open services.  
•	- Remove Apache and rerun `nmap`; reinstall and observe differences.    
•	- Enable UFW with `sudo ufw enable`, allow port 80, and observe service access.  
•	- Attempt `ssh [partner_ip]`, troubleshoot with UFW rules.  
•	- Create a new user: `sudo adduser username` and SSH using `ssh username@ip`.    
•	- Download books from Project Gutenberg using `wget`.  
•	- Create directory `books`, move files, create tar: `tar cf books.tar books`.  
•	- Compress with `bzip2 books.tar`, decompress with `bunzip2`, extract with `tar -xvf`.  
Challenge Activities
Challenge 1: Remote File Creation via SSH
•	- SSH into your partner’s machine and create a file on their Desktop.  
Challenge 2: Remote GUI Apps
•	- Attempt to launch `gedit` while SSH’ed in. Discuss why it may fail.  
Challenge 3: SCP File Transfer
•	- Use `scp file.txt user@host:/destination/` to send a file over the network.  
•	- Try to copy a directory of files using SCP recursively.  
Challenge 4: Compress & Share Books
•	- Download 10 books, compress with tar + bzip2, and SCP to your peer’s machine.
Virtual Networking
•	- Clone the VM in VirtualBox (must power off first).
•	- Add a NAT Network via File > Preferences > Network in VirtualBox.
•	- Set both VMs to use the same NAT network adapter.
•	- Boot both VMs and check IP with `ip a`.
•	- Fix MAC conflict if IPs are the same by regenerating MAC address.
•	- Ping between VMs and test SSH connectivity.
Reflection Questions
•	- What’s the role of a firewall in managing services?
•	- How did SSH access deepen your understanding of Linux as a server?
•	- Why is file compression important in server contexts?
•	- How does user privilege management help secure systems?



 
🛠️ Activity: Linux Services, Networking, and Secure File Transfers
📘 Objective
Set up and explore Apache, SSH, and UFW firewall services in Ubuntu, perform port scanning and file transfer over SSH, and practice compression and decompression using tar, bzip2, and scp.

📦 Deliverables
#	Deliverable	Description
✅ 1	Apache Web Server Installed	Screenshot or terminal output of sudo apt install apache2 and Apache running at http://127.0.0.1.
✅ 2	Modified index.html Page	Edited /var/www/html/index.html and screenshot showing personalized content when visited via browser or neighbor’s IP.
✅ 3	IP Address Identified and Shared	Output of ip a showing local and loopback IPs. Partner's IP exchanged and used to access each other's webserver.
✅ 4	Nmap Port Scan Results	Output screenshot of nmap [partner’s IP] showing open ports before and after Apache is removed.
✅ 5	Firewall (UFW) Status and Rules	Outputs of: 
• sudo ufw status verbose before and after enabling 
• Port 80 allowed and verified via partner’s Nmap scan
✅ 6	SSH Enabled and Tested	Output of successful login via ssh to partner’s machine using both default and explicitly declared usernames.
✅ 7	New User Created and Verified	Command and confirmation of user added via sudo adduser, with /etc/passwd showing new entry.
✅ 8	Compression and Decompression Tested	Screenshots of: 
• tar cf, bzip2, bunzip2, and tar -xvf 
• Output of ls -la showing archive size comparison
✅ 9	SCP File Transfers Between Machines	Output or screenshots showing successful use of scp to copy: 
• A file 
• A directory (bonus)
✅ 10	/etc/hosts File Modified	Screenshot showing added custom hostname (e.g., 8.8.8.8 GoogleEpicDNS) and successful ping GoogleEpicDNS.
✅ 11	nslookup and whois Commands Run	Output of: 
• nslookup google.com 
• whois google.com (after installing whois)
✅ 12	Public vs Private IP Comparison	Screenshot of ip a and result from https://whatismyipaddress.com, with short explanation.

✅ 13	Hardware Info Extracted	Output from: 
• lsusb 
• lspci 
• less /proc/cpuinfo with CPU core count identified.
✅ 14	Redirected Output Tested	Output file from: lsusb > output_of_lsusb, viewed using cat and less. File size shown using ls -la.
✅ 15	Extension Challenge 1 Completed	SSH into partner’s machine and create a file on their desktop: Hi_[partner’s name].
✅ 16	Extension Challenge 2 Completed	Attempt to launch gedit over SSH and note if successful. Explain result (X11 forwarding limitation or GUI requirement).
✅ 17	Extension Challenge 3 Completed	Use scp to copy multiple files between systems; include scp command used and success message or transfer log.
✅ 18	Extension Challenge 4 Completed (Bonus)	Download top 10 books from Gutenberg, compress them with tar and bzip2, then transfer to partner via scp.
✅ 19	Two VMs Networked (External/Online Students)	Output of ip a showing both VM IPs, successful ping, and ssh between cloned machines.
✅ 20	Reflection Paragraph (Optional)	A short reflection (100–200 words) on working with Linux networking, SSH, and file compression/transfers.

📝 Suggested Submission Format
•	A .zip file containing:
o	Screenshots (.png or .jpg)
o	Terminal outputs (.txt or screenshots)
o	Compressed archive (books.tar.bz2)
o	Reflection (.txt or .docx)
o	Any .c or .html files edited

