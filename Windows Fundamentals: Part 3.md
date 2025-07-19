
### **TryHackMe: Windows Fundamentals**

**Room:** `Part 3`  
**Status:** Completed  
**Date:** 2025-07-19

----------

### **Goal**

Develop an understanding of built-in Windows security features and tools, including Windows Update, Windows Security, Firewall configurations, exploit protection, BitLocker, and Volume Shadow Copy Service (VSS).

----------

### **Key Topics Covered**



**1. Windows Update**

-   Windows Update is a Microsoft service that provides patches, security updates, and feature improvements for Windows OS and Microsoft software like Defender.
    
-   Regular updates are released on the second Tuesday of each month ("Patch Tuesday"), with urgent updates pushed as needed.
    
-   Access via:
    
    -   _Settings_
        
    -   Command line: `control /name Microsoft.WindowsUpdate`
        

**2. Windows Security Dashboard**

-   A central hub for managing Windows protection tools.
    
-   Covers several protection areas:
    
    -   **2.1 Virus & Threat Protection**
        
    -   **2.2 Firewall & Network Protection**
        
    -   **2.3 App & Browser Control**
        
    -   **2.4 Device Security**
        

**2.1 Virus & Threat Protection**

-   Split into:
    
    -   _Current threats_: Scan options (quick, full, custom), threat history
        
    -   _Virus & threat protection settings_:
        
        -   **Real-time protection**: Blocks malware in real-time
            
        -   **Cloud-delivered protection**: Fast, cloud-based updates
            
        -   **Automatic sample submission**: Sends suspicious files to Microsoft
            
        -   **Controlled folder access**: Prevents unauthorized access to key areas
            
        -   **Exclusions**: Specify files/folders to skip in scans
            
        -   **Notifications**: Alerts on security activity
            

**2.2 Firewall & Network Protection**

-   Includes three profile types:
    
    -   **Domain network**
        
    -   **Private network**
        
    -   **Public network**
        
-   Each profile allows firewall toggling and blocking all incoming connections.
    
-   Advanced configuration available for experienced users via:
    
    -   Command: `wf.msc`
        

**2.3 App & Browser Control**

-   Configure Microsoft Defender SmartScreen:
    
    -   Warn, block, or ignore unknown/untrusted web apps and files.
        
-   **Exploit protection** settings:
    
    -   Protect against various attack vectors
        
    -   Examples:
        
        -   _Control Flow Guard_: Validates indirect calls
            
        -   _Data Execution Prevention_: Blocks code in data-only memory
            

**2.4 Device Security**

-   Focuses on:
    
    -   **Core Isolation > Memory Integrity**: Prevents code injection into secure processes (off by default)
        
    -   **Security Processor (TPM)**:
        
        -   Hardware-based crypto chip for secure operations
            
        -   Tamper-resistant, used in secure boot, BitLocker, and encryption
            

**3. BitLocker**

-   Encrypts drives to prevent data exposure/theft from lost or improperly disposed devices.
    
-   Works best with a TPM chip for secure key storage and system integrity checks.
    

**4. Volume Shadow Copy Service (VSS)**

-   Coordinates snapshot creation for consistent data backups.
    
-   Stored in the _System Volume Information_ folder.
    
-   Accessible via Advanced System Settings to:
    
    -   Create restore points
        
    -   Perform system restore
        
    -   Manage restore settings
        
    -   Delete restore points
        
-   Malware often targets VSS to prevent recovery during ransomware attacks, highlighting the importance of offline/off-site backups.
    

----------

### What I Learned

-   Windows offers layered, built-in security tools to protect both the system and user data.
    
-   Real-time protection, SmartScreen, and exploit mitigation contribute to a strong defense against common threats.
    
-   BitLocker and TPM provide hardware-level encryption and integrity checks.
    
-   Volume Shadow Copy enables rollback to restore points, but must be protected from malicious tampering.
    
-   Understanding how and where to access each tool enhances the ability to manage, troubleshoot, and secure a Windows environment.
