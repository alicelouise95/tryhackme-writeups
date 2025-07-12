## TryHackMe: HTTP in Detail

**Room**: HTTP in Detail  
**Status**: Completed  
**Date**: 2025-07-12

----------

### Goal

Understand the structure and function of HTTP, including requests, responses, status codes, headers, and cookies. Learn how web clients and servers communicate using these elements.

----------

### Key Topics Covered

#### 1. What is HTTP?

-   HTTP (HyperText Transfer Protocol) is the protocol used for transmitting data (HTML, images, video, etc.) between clients and web servers.
    
-   HTTPS is the secure version, encrypting data and authenticating the server.
    

----------

#### 2. Requests and Responses

-   **URL (Uniform Resource Locator)** is broken into parts like scheme, user info, host, port, path, query string, and fragment.
    
-   Basic HTTP request format
    
    `GET / HTTP/1.1 Host: tryhackme.com  User-Agent: Mozilla/5.0 Firefox/87.0  Referer: https://tryhackme.com` 
    
-   Basic HTTP response:
   
    `HTTP/1.1 200 OK Server: nginx  Content-Type: text/html  Content-Length: 98` 
    

----------

#### 3. HTTP Methods

-   **GET** – Retrieve data
    
-   **POST** – Submit data (create)
    
-   **PUT** – Update data
    
-   **DELETE** – Remove data
    

----------

#### 4. HTTP Status Codes

-   **100–199**: Informational
    
-   **200–299**: Success
    
-   **300–399**: Redirection
    
-   **400–499**: Client errors
    
-   **500–599**: Server errors
    

**Common Codes**:

-   200 – OK
    
-   201 – Created
    
-   301 – Moved Permanently
    
-   400 – Bad Request
    
-   401 – Unauthorized
    
-   403 – Forbidden
    
-   404 – Not Found
    
-   405 – Method Not Allowed
    
-   500 – Internal Server Error
    
-   503 – Service Unavailable
    

----------

#### 5. HTTP Headers

**Request Headers**:

-   `Host`: Target domain
    
-   `User-Agent`: Client/browser details
    
-   `Content-Length`: Size of body data
    
-   `Accept-Encoding`: Accepted compression formats
    
-   `Cookie`: Sends stored data to the server
    

**Response Headers**:

-   `Set-Cookie`: Stores data on client
    
-   `Cache-Control`: Caching rules
    
-   `Content-Type`: Data type (HTML, JSON, etc.)
    
-   `Content-Encoding`: Compression type
    

----------

#### 6. Cookies

-   Small pieces of data saved by the browser and sent with every request.
    
-   Set using the `Set-Cookie` response header.
    
-   Used to store sessions, preferences, and tracking info.
    

----------

### What I Learned

-   HTTP governs how web browsers and servers exchange information using requests and responses.
    
-   URLs contain structured components, and headers are essential for smooth communication.
    
-   Different HTTP methods exist for retrieving, sending, updating, and deleting data.
    
-   Status codes indicate the result of a request and help identify issues.
    
