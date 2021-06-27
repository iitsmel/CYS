**Specifically target a web to crack its user name and password.**

## Firefox Settings

1. Click the bar like thingy on the right
2. Click Options
3. Scroll down
4. Click Network Settings, Settings…
5. Change Config from “ Use system proxy settings “ to “ Manual proxy configuration “
6. Enter 127.0.0.1 to HTTP Proxy and 8081 to port ( port’s not 8080 cause it is used by file )
7. Check Also use this proxy for FTP and HTTP
8. Do not put anything in “ No proxy for “ box
9. Click OK
10. Go to about:config
11. Type in network.proxy.allow.hijacking_localhost and change it to true
12. Type in network.proxy.no_proxies_on to empty
13. Search for PortSwigger CA and download it
14. Open Option in Firefox again
15. Type in “ certificates “ in Find in Options box
16. Click View Certificates
17. Click Import
18. Click the CA just downloaded
19. Click Open
20. Click OK

## Burp ( community edition )

1. Temporary project
2. Next
3. Start Burp
4. Click Proxy —> Options
5. Check Interface for ip: port( 172.0.0.1;8081)
6. Check Intercept Client Requires, following rules
7. Check HTTP method ( Alter operator to And, relationship to Matches, condition to get. )
8. Check URL ( Alter condition to localhost. )
9. Check Auto update Content-Length blah
10. Check Intercept Server Responses, following rules
11. Click Intercept
12. Check Intercept is on
13. Connect Firefox to DVWA