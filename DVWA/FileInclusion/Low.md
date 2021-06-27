Click to see file1.php, file2.php and file3.php. It is showed from the URL that the last few words are changeable.

http:// ( where the file is stored or ip address )/DVWA/vulnerabilities/fi/( type in the things attackers want to find out )

If attackers typed in " /?page=/etc/shadow ", they will be able to obtain the absolute path of the document. Which is dangerous, because sometimes the attackers are aiming for valuable docs then they might be able to get it due to lack of security.

However the attackers are also might be able to get the access due this same issue.

( root files location might look like : /usr/share/doc )