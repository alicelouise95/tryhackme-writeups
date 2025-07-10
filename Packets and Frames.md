
### **TryHackMe: Packets & Frames**

**Room:** `Packets & Frames`  
**Status:** Completed  
**Date:** 2025-07-10

----------

### **Goal**

Understand how data is divided into smaller pieces and transmitted across a network to another device.

----------

### **Key Topics Covered**

**1. Packets vs. Frames**

-   Learned the difference between **packets** and **frames**.
    
-   **Frames** carry the actual data — once encapsulation layers are removed, the frame is what remains.
    
-   **Packets** contain IP-related information such as source and destination IP addresses.
    
-   If something references an IP address, it typically refers to a **packet**.
    

**2. Packet Structure and IP Headers**

-   Examined how packet structure varies by protocol (e.g., IPv4).
    
-   Looked at key fields in an IP packet:
    
    -   **Source IP / Destination IP**
        
    -   **Time to Live (TTL)**
        
    -   **Checksum** (for error detection)
        

**3. TCP/IP Model**

-   Compared it to the OSI model — TCP/IP has 4 layers:
    
    -   **Application**
        
    -   **Transport**
        
    -   **Internet**
        
    -   **Network Interface**
        
-   Understood that each layer adds headers during **encapsulation**.
    

**4. TCP Packets and the Three-Way Handshake**

-   Reviewed the components of a TCP packet:
    
    -   **Source/Destination Ports**
        
    -   **Sequence Number**
        
    -   **Acknowledgement Number**
        
    -   **Flags (e.g., SYN, ACK, FIN)**
        
    -   **Checksum**
        
-   Learned the **three-way handshake**:
    
    -   **SYN → SYN/ACK → ACK**
        
-   Covered how TCP sessions are closed (FIN, ACK...)
    

**5. UDP Overview**

-   Looked at how **UDP** differs from TCP:
    
    -   No session setup
        
    -   Faster, but less reliable
        
    -   Used in scenarios where speed is more important than reliability (e.g., video streaming)
        

**6. Ports and Common Protocols**

-   Learned common **protocols** and their **port numbers**:
    
    -   **HTTP** – Port 80
        
    -   **HTTPS** – Port 443
        
    -   **SSH** – Port 22
        
    -   **FTP** – Ports 20/21
        
    -   **SMB** – Port 445
        
    -   **DNS** – Port 53
        

----------

### **What I Learned**

-   Packets and frames represent different levels of network data.
    
-   Encapsulation adds structure to data at every layer.
    
-   TCP is connection-oriented and reliable, while UDP is faster and connectionless.
    
-   The three-way handshake is essential for establishing a TCP connection.
    
-   Port numbers are used to identify services on a device.
