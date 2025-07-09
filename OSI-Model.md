
### **TryHackMe: OSI Model**

**Room:** `OSI Model`  
**Status:** Completed  
**Date:** 2025-07-09

----------

### **Goal**

Understand the 7-layer OSI model and the specific functions of each layer in network communication.

----------

### **Key Topics Covered**

**1. Overview of the OSI Model**

-   OSI stands for Open Systems Interconnection.
    
-   It’s a model that outlines how devices communicate over a network.
    
-   It consists of 7 layers, each with different responsibilities.
    
-   Encapsulation is the process of data gaining extra information as it moves through each layer.
    

**2. Layer 1 – Physical**

-   Refers to the physical components of networking, such as Ethernet cables.
    
-   Data is transmitted using electrical signals in binary format (1s and 0s).
    

**3. Layer 2 – Data Link**

-   Handles physical addressing using MAC addresses.
    
-   Formats the data for transmission and ensures it’s sent to the correct physical device.
    

**4. Layer 3 – Network**

-   Focuses on IP addressing and routing.
    
-   Routes packets across networks using protocols like OSPF and RIP.
    
-   Chooses the most efficient path based on speed, reliability, and distance.
    

**5. Layer 4 – Transport**

-   Manages reliable data transfer using protocols like TCP and UDP.
    
-   **TCP**: Reliable, connection-oriented, error-checking, slower.
    
-   **UDP**: Faster, no guarantee of delivery, used for streaming and similar applications.
    

**6. Layer 5 – Session**

-   Establishes, maintains, and terminates communication sessions.
    
-   Responsible for managing the length and status of active connections.
    

**7. Layer 6 – Presentation**

-   Translates data between applications and the network.
    
-   Handles data format standardization and encryption.
    

**8. Layer 7 – Application**

-   Interface between the user and the network.
    
-   Handles application-specific protocols like HTTP, SMTP, etc.
    

----------

### **What I Learned**

-   The OSI Model helps break down complex networking processes into manageable layers.
    
-   Each layer is responsible for a specific part of how data is prepared, sent, and received.
    
-   TCP and UDP offer two distinct approaches to data transport depending on the use case.
    
-   Encapsulation is a central concept in how data is built as it travels through the stack.
