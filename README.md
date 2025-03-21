# FreePBX-Raspberry-Pi-Easy-Setup
A simple script to install FreePBX on Raspberry Pi

 I was trying to install an opensource VoIP PBX on my Raspberry, however, has no much resources and tutorials online to make this. I dont't know why it is so hard, but here is a solution. This script will allow you to install FreePBX on a Raspberry Pi without spending much time and brain connections. LOL :)

 Recomended Hardware:
```
Raspberry Pi 4 4gb
32gb MicroSD Card
Gigabit Ethernet
```


Before starting:
* Use root to login
* Open configurations with ```sudo raspi-config```
* Expand you filesystems in ```Advanced > Expand filesystem```
* Don't select to reboot now


Notice:
Some configs will be changed. They are:
 1. Timezone: ```Europe/London```
 2. Locale: ```en_GB.UTF-8```
 3. Hostname: ```raspbx```


To make things easier:

```
sudo apt update -y && sudo apt full-upgrade -y && sudo apt install git -y
sudo timedatectl set-timezone Europe/London
sudo hostname raspbx
sudo git clone https://github.com/theocastro/FreePBX-Raspberry-Pi-Easy-Setup.git
cd FreePBX-Raspberry-Pi-Easy-Setup
sudo chmod +x install
sudo ./install
```



Special thanks for
<br/>
```Mr. Scott Phillips (Script owner)```: https://sourceforge.net/u/thatguy/profile <br/>
```Unify Communications (Video Tutorial)```: https://www.youtube.com/watch?v=wXVLvxrEWeY&t=134s
