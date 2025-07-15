
### **TryHackMe: Linux Fundamentals**

**Room:** `Part 2`  
**Status:** Completed  
**Date:** 2025-07-15

----------

### **Goal**

Learn how to remotely access Linux systems via SSH, understand common command flags and switches, manage files and directories, explore permission systems, and get familiar with important system folders.

----------

### **Key Topics Covered**

**1. SSH (Secure Shell)**

-   SSH is a secure protocol used to access and control remote machines over a network.
    
-   It uses encryption to ensure that data transferred between the local and remote device remains confidential.
    
-   Logged into a TryHackMe machine using the syntax: `ssh tryhackme@<IP_ADDRESS>`.
    
-   Required both the remote IP and valid login credentials.
    
-   On first connection, had to confirm trust of the host before entering the password.
    

**2. Flags and Switches**

-   Explored command flags using the manual (`man`) and `--help`.
    
-   Learned how flags modify command behavior:
    
    -   `ls -a`: shows hidden files.
        
    -   `ls -l`: displays detailed file info.
        
    -   `ls -lh`: adds human-readable file sizes.
        
-   Practiced checking documentation and experimenting with flags in the terminal.
    

**3. Filesystem Interaction (Continued)**

-   Learned to create, move, copy, and delete files and directories:
    
    -   `touch`: create file
        
    -   `mkdir`: create directory
        
    -   `cp`: copy
        
    -   `mv`: move/rename
        
    -   `rm`: remove
        
    -   `file`: check file type
        
-   Practiced working with different types of files and navigating the system.
    

**4. Permissions 101**

-   Every file has permissions for **owner**, **group**, and **others**: read (`r`), write (`w`), and execute (`x`).
    
-   Groups allow multiple users to share access to the same file with specific permission levels.
    
-   Used `su` to switch users.
    
    -   Needed the target username and password.
        
    -   `su -l`: starts a full login shell, inheriting environment variables.
        

**5. Common Directories**

-   `/etc`: stores system configuration files (e.g., `sudoers`).
    
-   `/var`: holds data written frequently by apps/services (e.g., `/var/log`).
    
-   `/root`: the root user's home directory.
    
-   `/tmp`: a temporary, writable directory cleared on reboot. Useful for storing tools during pentesting.
    

----------

### **What I Learned**

-   SSH enables secure, remote access to Linux machines.
    
-   Command flags extend basic command functionality for better control and output.
    
-   File management in Linux is intuitive and powerful using core CLI tools.
    
-   Understanding permissions and users is key to secure and organized systems.
    
-   Certain system folders hold configuration files, logs, and temporary data vital to both administration and pentesting.
