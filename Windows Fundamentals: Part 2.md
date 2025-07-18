
### **TryHackMe: Windows Fundamentals**

**Room:** `Part 2`  
**Status:** Completed  
**Date:** 2025-07-18

----------

### **Goal**

Explore key Windows system utilities used in diagnostics and administration, including the System Configuration utility, Event Viewer, Task Scheduler, Device Manager, and more.

----------

### **Key Topics Covered**

1.  **System Configuration Utility (msconfig)**
    
    Used for advanced diagnostics and troubleshooting.
    
    Requires administrator privileges to open.
    
    Includes five tabs:
    
    -   **General** – Choose startup mode (Normal, Diagnostic, Selective).
        
    -   **Boot** – Configure OS boot options and safe boot settings.
        
    -   **Services** – Enable/disable background services.
        
    -   **Startup** – Shortcut to Task Manager’s Startup tab.
        
    -   **Tools** – Launch various built-in administrative tools.
        
2.  **User Account Control (UAC) Settings**
    
    Allows users to define when Windows should notify them before changes are made that require admin permissions.
    
    Options range from "Always notify" to "Never notify" (not recommended).
    
    Helps mitigate malware by restricting silent elevation of privileges.
    
3.  **Computer Management (compmgmt.msc)**
    
    Centralized interface that includes multiple Windows tools under one window.
    
    Divided into three main categories:
    
    -   **System Tools**
        
    -   **Storage**
        
    -   **Services and Applications**
        
4.  **Task Scheduler**
    
    Allows automation of tasks based on triggers (e.g., user logon, system idle).
    
    Useful for scheduled maintenance, backups, and script execution.
    
    Tasks can be configured with conditions and actions, such as launching programs.
    
5.  **Event Viewer**
    
    Displays detailed logs from system, security, and application events.
    
    Key log categories:
    
    -   **Application** – Software-related events.
        
    -   **Security** – Logins, logoffs, audit failures.
        
    -   **System** – Driver load failures, shutdowns, restarts.
        
    
    Event types include:
    
    -   **Error** – Critical issues (e.g., data loss).
        
    -   **Warning** – Non-critical but noteworthy problems.
        
    -   **Information** – Successful operations.
        
    -   **Audit Success/Failure** – Security-related logging (login attempts, etc.).
        
6.  **Device Manager**
    
    Provides access to hardware configuration and driver status.
    
    Devices are categorized (e.g., Display adapters, Network adapters).
    
    Allows:
    
    -   Updating, disabling, or uninstalling drivers.
        
    -   Viewing device properties and error codes.
        
7.  **System Information (msinfo32)**
    
    Displays a detailed summary of hardware, system components, and software environment.
    
    Includes:
    
    -   OS version and build.
        
    -   System manufacturer and model.
        
    -   BIOS version.
        
    -   Memory and CPU info.
        
    -   Driver and service details.
        
8.  **Resource Monitor (resmon)**
    
    Provides real-time monitoring of system resources:
    
    -   **CPU** – Active processes and services.
        
    -   **Memory** – Usage, faults, and allocation.
        
    -   **Disk** – Read/write activity by file and process.
        
    -   **Network** – Current connections and traffic.
        
9.  **Performance Monitor (perfmon)**
    
    Used to track and log performance metrics over time.
    
    Metrics can be added to custom Data Collector Sets.
    
    Supports graphs and reports for analysis.
    
    Can be useful for diagnosing performance bottlenecks.
    

----------

### What I Learned

-   The **System Configuration Utility** provides a simplified gateway to advanced diagnostics and selective startup.
    
-   Tools like **Task Scheduler** and **Event Viewer** are invaluable for understanding and automating system behavior.
    
-   **Device Manager** and **System Information** offer insights into hardware health and compatibility.
    
-   **Resource Monitor** and **Performance Monitor** allow for deep visibility into real-time and historical system performance.
    
-   Collectively, these tools form the backbone of effective system administration and troubleshooting in Windows.
