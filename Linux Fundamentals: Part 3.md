
### **TryHackMe: Linux Fundamentals**

**Room:** `Part 3`  
**Status:** Completed  
**Date:** 2025-07-16

----------

### **Goal**

Gain practical experience with Linux process management, automation via cron jobs, package management, service control, and log analysis.

----------

### **Key Topics Covered**


**1. Terminal Text Editors**

-   Practiced using `nano` and `vim` to create and edit files directly in the terminal.
    
-   `nano` is beginner-friendly; `vim` is more advanced but powerful once mastered.
    
-   Used keyboard shortcuts to save (`Ctrl+O`) and exit (`Ctrl+X` in nano, `:wq` in vim).
    

**2. File Transfer with `wget` and HTTP Server**

-   Used `wget` to download files from a remote server: `wget http://<IP>:8000/filename`.
    
-   Created a quick file server using Python: `python3 -m http.server`.
    
-   Useful for transferring scripts or tools during CTFs or pentesting.
    

**3. Process Management**

-   Explored running processes using `ps`, `ps aux`, and `top`.
    
-   Every process has a unique PID (Process ID).
    
-   Sent signals to control processes using `kill`, including:
    
    -   `SIGTERM` – graceful stop
        
    -   `SIGKILL` – force stop
        
    -   `SIGSTOP` – pause execution
        

**4. `systemd` and Namespaces**

-   Learned that `systemd` is the init system (PID 1) responsible for booting and managing services.
    
-   Introduced to Linux namespaces, which isolate process trees, filesystems, and more.
    
-   `systemd` launches services into isolated namespaces during system startup.
    

**5. Managing Services with `systemctl`**

-   Used `systemctl` to manage services:
    
    -   `start`, `stop`, `restart`
        
    -   `enable`, `disable` (for persistence on boot)
        
-   Example: `systemctl start apache2` starts the Apache web server.
    

**6. Foreground and Background Processes**

-   Ran processes in the background with `&`.
    
-   Suspended processes using `Ctrl + Z`.
    
-   Brought jobs back with `fg`.
    
-   Verified backgrounded jobs using `ps`.
    

**7. Automation with `cron` and `crontab`**

-   Used cron jobs to schedule repeating tasks.
    
-   Edited cron schedules with `crontab -e`.
    
-   Understood cron syntax:
    
    -   `0 */12 * * *` → runs every 12 hours
        
-   Common for backups, monitoring scripts, and maintenance tasks.
    

**8. APT Package Management**

-   Installed software using `apt install <package>`.
    
-   Added new software sources by editing `/etc/apt/sources.list.d/`.
    
-   Imported GPG keys with `apt-key add`.
    
-   Removed software with `apt remove` and cleaned repos manually if needed.
    

**9. Logs and Monitoring**

-   Found Apache logs under `/var/log/apache2/`.
    
-   Viewed logs using `cat`, `less`, or `tail -f`.
    
-   Logs help detect errors, attacks, and system events.
    

----------

### **What I Learned**

-   How to edit files within the terminal using `nano` and `vim`.
    
-   File transfer with `wget` and a Python HTTP server is quick and effective.
    
-   Understanding and controlling processes is vital for system management.
    
-   `systemd` is key to managing services and boot procedures.
    
-   Cron jobs allow automation of routine tasks.
    
-   APT package management simplifies software installation and updates.
    
-   System logs provide critical insight for debugging and auditing.

