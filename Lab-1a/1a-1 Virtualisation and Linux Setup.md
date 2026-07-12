Lab-1a Installing VMware and Ubuntu

1\. Installed VMware on host OS (Windows 11). would show the VMware application installed and visible in the Start Menu.  
![VMware Installed](Lab-1a/1-a 1 VMware Installed.png)
2\. Downloaded Ubuntu 22.04.3 LTS ISO image from the official Ubuntu website. Screenshot would show the downloaded file (ubuntu-22.04.3-desktop-amd64.iso).  



3\. Created a new Virtual Machine in VMware named 'Ubuntu-Lab1a' with 2048 MB RAM and 20 GB disk. Screenshot would show VM settings (RAM, boot order, ISO mounted).   

4\. Booted VM using ISO and installed Ubuntu. Screenshot would show successful login screen of Ubuntu desktop.

&#x20;

Ran into this issue when booting up VM, had to configure settings in BIOS to enable SVM  

&#x20;

5\. Configured network settings in VMware using NAT mode. Screenshot would show VMware Network settings page with NAT selected, 

 

6\. Verified Ubuntu running with GUI access. Screenshot would show Ubuntu desktop with Terminal open.

&#x20;

7\. Installed VMware tools inside Ubuntu. Evidence would include successful execution of `sudo apt install open-vm-tools-desktop -y` and reboot.  

8\. Enabled SSH server (advanced option). Screenshot would show `sudo apt install openssh-server` and `systemctl status ssh` confirming active service.  

9\. Alternative path: Installed WSL Ubuntu from Microsoft Store (Windows 11). Screenshot would show Ubuntu running in PowerShell with `ls` command output.

10\. Bonus exploration: Installed Fedora Workstation 38 in a separate VM. Screenshot would show Fedora desktop login screen.

Deliverables

✅ VMware Installed – Screenshot of installation complete.

✅ Ubuntu ISO Downloaded – Screenshot of ISO file in Downloads folder.

✅ VM Created – Screenshot of VM configuration.

✅ Ubuntu Installed – Screenshot of Ubuntu desktop/terminal.

✅ Networking Configured – Screenshot of VMware NAT/Bridged settings.

✅ Ubuntu Running – Screenshot of terminal/desktop proving functionality.

✅ VMware Tools Installed – Screenshot or command output of installation.

✅ SSH Enabled – Screenshot of SSH service status.

✅ Alternate: WSL Installed – Screenshot of Ubuntu running on Windows terminal.

✅ Bonus: Other Distro Explored – Screenshot of Fedora/Kali/Debian installed.



