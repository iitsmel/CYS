## Start Brutal Force level low.

1. Open xampp and start Apache n MYSQL.
2. Type “ admin “ in username, anything but “ password “ in password.
3. After Burp successfully connect to DVWA, click Forward
4. Click Action, Send to Intruder
5. Click Intercept is on, turn it off
6. Click Intruder
7. Click Positions
8. Click Clear on the right
9. Double click admin( the word after username = )
10. Click Add
11. Double click the random word ( the word after password = )
12. Click Add
13. Click Attack type chose Cluster bomb
14. Click Payloads
15. Chose Payload set to 1
16. Chose Payload type to Simple list
17. Click the box on the right of Add under Payload Options [ Simply list ]
18. Type in anything, it’s for brutal force cracking username
19. Click Add to add it to combination
20. Click Payload set to 2
21. Click the box on the right of Add under Payload Options [ Simply list ]
22. Type in anything, it’s for brutal force cracking password
23. Click load to choose a txt file which might full of password combinations made by you
24. Click Options
25. Scroll down to Grep-Match
26. Clear the box
27. Go to DVWA page
28. Click View Source at the corner of lower right
29. Scroll down and copy “ Username and/or password incorrect. “
30. Back to Burp
31. Paste it in the box on the right of Add
32. Click Clear first to clear the default error message
33. Click Add, Add it to the box
34. Scroll up and click Start Attack
35. Find the one which isn’t checked on User…
36. Payload 1 n Payload 2 are the right combo of username and password
37. Go back to DVWA
38. Type in the right username and password