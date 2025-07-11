### **TryHackMe: DNS in Detail**

**Room:** `DNS in Detail`  
**Status:** Completed  
**Date:** 2025-07-11

----------

### **Goal**
Understand how the Domain Name System (DNS) functions, including its structure, record types, and the process by which domain names are resolved to IP addresses.

----------

### Key Topics Covered

#### 1. What DNS Is

DNS is responsible for translating human-readable domain names (like `tryhackme.com`) into numerical IP addresses that computers use to route traffic and communicate.

----------

#### 2. Domain Hierarchies

-   **Root Domain (`.`)** – Top of the DNS structure.
    
-   **TLD (Top-Level Domain)** – The rightmost part of a domain (e.g., `.com`, `.org`, `.co.uk`).
    
    -   `gTLD` – Generic (e.g., `.com`, `.org`)
        
    -   `ccTLD` – Country-code (e.g., `.uk`, `.se`)
        
-   **Second-Level Domain** – The main part of the domain (e.g., `tryhackme` in `tryhackme.com`)
    
-   **Subdomain** – Prefix added to a domain (e.g., `admin.tryhackme.com`)
    

----------

#### 3. DNS Record Types

-   **A Record** – Points to an IPv4 address
    
-   **AAAA Record** – Points to an IPv6 address
    
-   **CNAME** – Alias of another domain (e.g., `store.tryhackme.com` → `shops.shopify.com`)
    
-   **MX Record** – Defines which mail servers handle email for the domain
    

----------

#### 4. How DNS Resolution Works

1.  **Local Cache** – Device checks its cache for a previously resolved address.
    
2.  **Recursive DNS Server** – Often provided by the ISP; looks in its own cache or performs a recursive query.
    
3.  **Root Server** – Points to the appropriate TLD server.
    
4.  **TLD Server** – Refers the query to the authoritative nameserver for the domain.
    
5.  **Authoritative DNS Server** – Delivers the final IP address back to the recursive resolver, which then returns it to the original requester.
    

-   Results are cached locally for a period defined by **TTL (Time to Live)**.
    

----------

### What I Learned

-   DNS is hierarchical and structured in a way that breaks domain names down into manageable layers.
    
-   The process of resolving a domain involves several types of servers working together: recursive, root, TLD, and authoritative.
    
-   Caching is crucial to improving DNS performance and reducing query times.
    
-   DNS record types each serve different purposes — especially important are A, AAAA, CNAME, and MX records.
    
