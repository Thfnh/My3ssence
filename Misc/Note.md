1. php-reverse-shell (upload function).
2. react2shell (CVE-2025-55182).
3. bash shell.
4. MariaDB default user: root.
5. check /.git; /robots.txt; /sitemap.xml.
6. HTTP1.1 -> check HTTP Request Smuggling.
7. Breaking Unauthorized by 'Change Request Method' in burp (check by changing HTTP method request. e.g.: POST-> POSTX, TRACE, ...).
8. Bypass two-factor authentication (2FA) by dropping the 2FA check request in Burp Intercept.
9. backlash (\\) in JavaScript can escape single or double quote (', ") when testing for XSS bypass.
10. Use hyphens (-) as arithmetic operators to chain payloads and break out of JavaScript string contexts without triggering syntax errors.
* ex: For 9. and 10. : var searchTerms = '\\\\' - alert()//'
* \&apos; ->   ' 
* \&quot; ->   "
* \&lt;   ->   <
* \&gt;   ->   >

11. Template literal (Sign: `... 'backtick' ...`): You can perform calculations or call functions directly inside the ${...} syntax. 
12. An input accepts JSON; try testing it with XML.
13. Appending a tilde ~ at the end of a PHP file name is a common technique attackers use to try to access backup or temporary files created by text editors or version control systems
14. Try changing http request to bypass csrf token validation.
15. HTTP Header Injection (search term: /?search=) !??!?