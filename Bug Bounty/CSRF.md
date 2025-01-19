CSRF stands for ~={red}Cross-Site Request Forgery=~ It's a security vulnerability where unauthorized commands are submitted
 from a user that the web application trusts. Here's a brief explanation:

1.  __CSRF__ attacks exploit trust relationships between websites.

2. They allow attackers to perform actions on behalf of users without their knowledge or consent.

3.~={green} Common examples include=~ :
   - Adding items to a shopping cart
   - Changing account settings
   - Transferring funds

4. ~={green}To prevent CSRF attacks=~ :
   - Use CSRF tokens in forms
   - Implement proper session management
   - Validate requests using same-origin policy

5. ~={green}Popular libraries for CSRF protection include=~ :
   - Django's django.middleware.csrf.CsrfViewMiddleware
   - Spring Security's CsrfFilter

6. ~={green}When implementing CSRF protection=~ :
   - Generate unique tokens for each request
   - Store tokens securely (e.g., in session)
   - Verify tokens on server-side before processing requests

7. Always validate that incoming requests originate from your website's domain.

CSRF protection is crucial for maintaining the security of web applications, especially those handling sensitive
 operations.
 ![[csrf-attack.png]]