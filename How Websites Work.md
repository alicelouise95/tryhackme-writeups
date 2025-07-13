## TryHackMe: How Websites Work

**Room**: How Websites Work
**Status**: Completed
**Date**: 2025-07-13


----------

### Goal

Understand how websites function at a basic level, including the relationship between browsers, servers, HTML/CSS/JS, and the potential vulnerabilities that can arise when data is not properly handled.

----------

### Key Topics Covered

#### 1. Data Flow: Browser to Server

  A diagram explains how a website works. The browser sends a request through the internet to the web server, and the web server responds through the internet and back to the browser.  

Two main components of a website were introduced:
    

-   Front End (Client Side): What the browser renders for the user to see and interact with.
    
-   Back End (Server Side): The server-side logic that processes requests and returns responses.
    

----------

#### 2. HTML and CSS

  Reviewed HTML, which defines the structure of a webpage, and CSS, which controls its styling and visual presentation.  
    A practical task involved fixing a broken line of HTML and adding an additional image:
    

-   Fixed: `<img src='img/cat-2.jpg'>` (was missing .jpg)
    
-   Added: `<img src='img/dog-1.png'>`
----------

#### 3. JavaScript

JavaScript is used to make websites interactive. Without it, pages would remain static.  

  A demo task required two changes:    

-   Set the content of an element with the ID "demo" to "Hack the Planet" using JavaScript.
    
-   Added a button that, when clicked, changed the text to "Button Clicked".  

    Final working code:
    
-   `<script type="text/javascript">document.getElementById("demo").innerHTML = "Hack the Planet"</script>`
    
-   `<button onclick='document.getElementById("demo").innerHTML = "Button Clicked";'>Click Me!</button>`
    
----------

#### 4. Sensitive Data Exposure

Sensitive data exposure happens when developers leave clear-text credentials or other private data in frontend code.  

- A task involved inspecting the source code of a mock login form. It contained test credentials inside a comment:  

`<!-- TODO: Remove test credentials! Username: admin Password: testpasswd -->`
  
   
----------

#### 5. HTML Injection

HTML injection occurs when a website does not sanitize user input and that input is reflected in the webpage. This can allow attackers to inject HTML code.  

In a demo task, inputting the following triggered an HTML injection vulnerability:  
`<a href="http://hacker.com">Alice</a>`  

The page then displayed “Welcome Alice” as a clickable link to an external malicious site.

----------

### What I Learned

-   Websites are made up of two key parts: the front end (what users see) and the back end (server-side processing and logic).
    
-   The browser communicates with a web server via HTTP requests and responses, passing through the internet in both directions.
    
-   HTML structures a webpage, CSS styles it, and JavaScript makes it interactive.
    
-   JavaScript can dynamically alter webpage content and respond to user interactions like button clicks.
    
-   Sensitive data (like login credentials) can be unintentionally exposed in source code comments and must always be removed before deployment.
    
-   HTML injection is a real vulnerability that occurs when user input is not properly sanitized—attackers can exploit this to inject their own code or links. Input validation and sanitization are crucial to website security.
    
