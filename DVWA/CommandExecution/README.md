**The web might block specific commands.**

## Reverse Shell

Netcat :

Basically a Linux system command but can also use in Windows and MacOS.

This is a utility that establish a TCP ( Transmission Control Protocol ) or UDP ( User Data Protocol ) connection between 2 computers, meaning it can write and read through an open port. With the help of the program, files can be transferred and commands can be executed in some instances.  Netcat can also use by server administrator.

In short terms, it can use by attackers to track your work after you've  been attacked and you realize it.

Another advantage is that you can copy files over network without having an FTP server, HTTP or any other service that allows data to be transmitted, no matter the file is small or big.

The netcat utility is used it create client-to-server connections. It can fulfill both server and client role.

To create a server that LISTENS to connections on the TCP port 4444 we run the command :

user @ server: ~ # netcat -l 4444

The -l parameter means that netcat is in listen ( server ) mode, and 4444 is the port that it is listening to. The terminal will remain on hold for a client to connect to the open server with netcat. If the need of verify that host service listen on port 4444 is in need, open a new terminal to the host station and run the command :

user @ server: ~ # netstat -tlnp

Active Internet Connections ( only server ) :

The netstat command display TCP services waiting for local station connections. We notice that the netcat program listens on port 4444.  the options of the netscat command are :

t – displays TCP connections

l – shows the services that are waiting for (listen) connections

n – disables name resolution for IP addresses and ports; we typically disable name resolution to eliminate the latency of the resolving process;

p – displays the name and PID of the network service process that awaits connections on the given port.

In construction display 0.0.0.0:4444 in the Local Address column means that the service listens to connections on all IP addresses/system interfaces available on port 4444.