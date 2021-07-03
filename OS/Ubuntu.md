# Ubuntu
## Environment
- Oracle VM VirtualBox 6.1 version
- Ubuntu 20.04.2.0

<br>

## VBoxGuestAddtions.iso
**"gcc make perl dkms" problem**

type in <br>

``
sudo apt-get update
``

``
sudo apt-get install build-essential gcc make perl dkms
``

``
reboot
``

Power off the machine.<br>

Go to Settings --> Storage --> remove VBoxGuestAddtions.iso --> click ok.<br>

Go to Settings's Storage --> click Controller:IDE --> click Optical Drive --> click Leave Empty.<br>

Start<br>

Go to Device and click "Insert Guest Additions CD image...".<br>

Click Run and enter password.<br>

Power off the machine.<br>

Start<br>

Done :)

