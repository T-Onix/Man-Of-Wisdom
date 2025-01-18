XSS stands for Cross-Site Scripting. It's a security vulnerability found in web applications 

- __Example__ : attackers inject malicious scripts into trusted websites. When users visit these sites, their browsers execute the malicious scripts, allowing attackers to steal information, hijack user sessions, or perform other harmful actions

#### There are three main types of XSS:

1. __Stored XSS__ : The malicious script is stored on the target server, such as in a database, and executed when a user accesses the infected content

2. __Reflected XSS__ : The script is reflected off a web server, such as in a search result or error message, and executed immediately

3. __DOM-based XSS__ : The vulnerability exists in the client-side code, and the malicious script is executed directly by the browser without involving the server

Preventing XSS involves practices like sanitizing and validating user input, using secure coding techniques, and employing Content Security Policies (CSP)

![[Xss.png]]

- ### Example
1. [[Xss-Script]]



