
### **TryHackMe: Windows Fundamentals**

**Room:** `Part 1`  
**Status:** Completed  
**Date:** 2025-07-17

----------

### **Goal**

Gain foundational knowledge of the Windows operating system, including its history, graphical interface, file system structure, user accounts, system folders, and basic system tools.

----------

### **Key Topics Covered**



**1. History and Editions of Windows**

-   Learned about the evolution of Windows OS versions, such as the popularity of **Windows XP** and the poor reception of **Windows Vista**.
    
-   Reviewed **end-of-life dates** for different versions, including Windows 10.
    
-   **Windows 11** comes in two editions: **Home** and **Pro**.
    
    -   The **Pro edition** includes **BitLocker Drive Encryption**, which enhances security if a device is lost or stolen.
        

----------

**2. Windows Graphical User Interface (GUI)**

-   The Windows GUI consists of elements such as the **desktop**, **start menu**, **taskbar**, **search box**, **task view**, **toolbars**, and **notification area**.
    
-   The **desktop** holds shortcuts to files, folders, and programs. Its appearance and organization can be customized through display settings.
    
-   The **start menu** has evolved visually, replacing the word "Start" with the Windows logo, but retains similar functionality.
    
    -   Key sections include:
        
        -   Account-related actions
            
        -   Shortcuts to folders (Documents, Pictures)
            
        -   Settings (gear icon)
            
        -   Power options (shutdown, sleep, restart)
            
        -   Recently added apps and alphabetically sorted apps
            
        -   **Tiles** for pinned apps/utilities (e.g., browser, mail, photos)
            
-   The **taskbar** displays any open programs, folders, or files.
    
-   The **notification area** shows the date/time and system icons like volume and network. Icons can be added/removed via taskbar settings.
    

----------

**3. File System (NTFS)**

-   Modern Windows uses **NTFS** (New Technology File System); earlier versions used **FAT16**, **FAT32**, and **HPFS**.
    
-   **FAT** is still common in USB drives and memory cards but not in standard Windows installations.
    
-   NTFS is a **journaling file system**, capable of self-repair using log data in case of failure.
    
-   NTFS supports **file/folder permissions**:
    
    -   Permissions like full control, modify, read, write, etc.
        
    -   Viewable via: Right-click > Properties > Security tab.
        
-   Introduced to **Alternate Data Streams (ADS)**:
    
    -   Allows multiple data streams per file.
        
    -   Used by malware to hide data, but also for legitimate metadata (e.g., marking internet downloads).
        
    -   Viewable using PowerShell.
        

----------

**4. System32 Folder & Environment Variables**

-   **System32** is a critical Windows folder that contains system files and stores **environment variables**.
    
-   Environment variables include:
    
    -   OS path
        
    -   Number of processors used
        
    -   Temporary folder location
        

----------

**5. User Accounts, Profiles, and Permissions**

-   Two main account types:
    
    -   **Administrator** – full system control (add users, install software, change settings).
        
    -   **Standard User** – limited to personal file/folder changes.
        
-   User accounts can be managed via:
    
    -   Start menu search
        
    -   System Settings (admin-only options)
        
    -   `lusrmgr.msc` (Local Users and Groups management)
        
-   Each user gets a **profile folder** in `C:\Users`, created during first login.
    
-   Users inherit permissions based on their **group memberships**, which are assigned by the administrator.
    

----------

**6. User Account Control (UAC)**

-   Introduced to reduce the risk of system compromise due to elevated privileges.
    
-   **UAC** requires confirmation for tasks needing elevated access, even for administrator accounts (excluding the built-in local admin).
    
-   Helps prevent malware from running unchecked under privileged accounts.
    

----------

**7. Settings vs Control Panel**

-   **Settings**: Simplified interface for common configuration tasks.
    
-   **Control Panel**: Offers more advanced and legacy system settings.
    
-   Some tasks bridge both, e.g., Network & Internet > Change Adapter Options leads to the Control Panel.
    

----------

**8. Task Manager**

-   **Task Manager** provides insight into:
    
    -   Processes
        
    -   Performance
        
    -   Users
        
    -   Startup programs
        
    -   Services
        
    -   System details
        
-   Allows control over **startup applications**.
    
-   Displays **last BIOS time**, which shows how long it took to initialize hardware during boot.
    

----------

### **What I Learned**

-   The Windows OS has gone through major changes in design, functionality, and reliability over the years.
    
-   Understanding the GUI layout and navigation is crucial for both usability and troubleshooting.
    
-   NTFS brings resilience and control over the file system, supporting permissions and metadata streams.
    
-   User management and group-based permissions are essential for maintaining a secure Windows environment.
    
-   System tools like UAC and Task Manager are valuable for maintaining control, visibility, and security.
