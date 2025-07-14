## TryHackMe: How Websites Work: Final Room

**Room**: Putting it all Together    
**Status**: Completed    
**Date**: 2025-07-14    
 
----------

### Goal

To consolidate everything learned in the “How the Web Works” module by understanding the full request lifecycle of a website, the role of supporting components like load balancers and CDNs, and how web servers deliver content.

----------

### Key Topics Covered

1.  **How a Website Request Works**  
    When you type a website URL into your browser, your computer needs the server’s IP address to proceed. It checks locally first, and if not found, queries DNS servers to resolve it. Once the IP is known, your browser sends an HTTP request to the web server, which then responds with the code to render the site in your browser.

    
2.  **Other Web Components**  
    Several components support and enhance web functionality:
    

-   **Load Balancers** distribute traffic across multiple servers to manage load and ensure uptime. Common algorithms include:
    
    -   _Round-robin_: sends each request to the next server in a list.
        
    -   _Weighted_: evaluates which server is least busy before sending the request.
        
    -   Load balancers also perform **health checks** to ensure servers are functioning.
        
-   **CDNs (Content Delivery Networks)** host static files (CSS, JS, images) across global servers. A user’s request is routed to the nearest CDN node, improving speed and performance.
    
-   **Databases** store and retrieve dynamic data for web applications. Examples include MySQL, PostgreSQL, MongoDB, and MSSQL.
    
-   **WAFs (Web Application Firewalls)** protect against common attacks by analyzing HTTP requests and filtering out malicious traffic through rate limiting and pattern detection.
    

3.  **How Web Servers Work**  
    Web servers listen for incoming connections using HTTP. Common software includes Apache, Nginx, IIS, and Node.js.
    

-   **Root Directory**:
    
    -   Linux: `/var/www/html`
        
    -   Windows: `C:\inetpub\wwwroot`
        
    -   Example: A request to `http://example.com/pic.jpg` is served from the root directory as `/var/www/html/pic.jpg`.
        
-   **Virtual Hosts**: Allow one server to host multiple websites by mapping different domain names to different root directories, e.g.:
    
    -   one. com → `/var/www/website_one`
        
    -   two. com → `/var/www/website_two`
        
-   **Static vs Dynamic Content**:
    
    -   _Static Content_: Files that do not change—e.g., HTML pages, images.
        
    -   _Dynamic Content_: Changes based on user interaction or data—e.g., a blog’s homepage updating with new posts. This content is generated using back-end languages like Python, Node.js, Ruby, etc. Dynamic content increases security risks if input isn’t handled properly.
        

4.  **Final Quiz – The Request Lifecycle**  
    The final task was a practical test on the full request process. The correct order of operations was:
    
 i.  Request tryhackme.com in your browser
    
 ii.  Check local cache for IP address
    
 iii. Check your recursive DNS server for address
    
 iv.  Query root server to find authoritative DNS server
    
 v.  Authoritative DNS server advises the IP address for the website
    
 vi.  Request passes through a web application firewall
    
 vii.  Request passes through a load balancer
    
 viii.  Connect to web server on port 80/443
    
 ix.  Web server receives the GET request
    
 x.  Web application talks to database
    
 xi.  Your browser renders the HTML into a viewable website

----------

### What I Learned

-   The complete end-to-end flow of a website request, from browser input to rendered content.
    
-   How DNS resolution, firewalls, load balancers, and CDNs work together to deliver web content efficiently and securely.
    
-   How web servers differentiate between static and dynamic content, and how virtual hosting allows for multiple websites on a single machine.
    
-   How back-end interactivity adds complexity and potential vulnerabilities to web applications.
    
-   The importance of infrastructure in scaling websites and protecting them from attacks.
    
