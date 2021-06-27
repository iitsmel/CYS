## Using DVWA under a virtual reality system.

In my case, cause I use personal hotspot so I do not need one. Normally you will need a VMware to create a " VR environment ", which means after you download VMware, you need to download a ISO file and mounted the ISO file( make it useable ) and set the specific ISO file to your main VR environment. Because DVWA is dame vulnerable so running it under VR is a more security way.

## Using DVWA by xampp

I use this. First of all I changed the config.txt file in config, changing its port to 8080, cause due to port issue if I didn't change it, it would cause the Apache fail starting. After changing that, I deleted all the files " htdocs ".

Terminal:

cd Desktop

cd xmapp

cd /opt/lampp/

cd ./manager-linux-x64.run

To open xampp

## FIERFOX

I changed some of the Firefox setting. Imma leave the explain to tacks section.

Firefox exr edition

## DVWA

First of all, I put the DVWA file under xampp file and put it in htdocs. After that, I opened the config file I change the password from "password" to "".

In order to start DVWA, I start the Apache and MySQL. Opening Firefox is clearly the next step, then I typed in " localhost:8080 ". Under the file, I found my DVWA and I clicked it in. Enter the user as " admin " and password as " password ". It should be all set by this time, g2g.