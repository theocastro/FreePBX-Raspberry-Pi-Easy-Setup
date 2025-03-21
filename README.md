# FreePBX-Raspberry-Pi-Easy-Setup
A simple script to install FreePBX on Raspberry Pi

 I was trying to install an opensource VoIP PBX on my Raspberry, however, has no much resources and tutorials online to make this. I dont't know why it is so hard, but here is a solution. This script will allow you to install FreePBX on a Raspberry Pi without spending much time and brain connections. LOL :)

 Recomended Hardware:
```
Raspberry Pi 4 4gb
32gb MicroSD Card
Gigabit Ethernet
```

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

Tips:
Use root to login, set locale to "en_GB.UTF-8" and expand filesystem.



Special thanks for
  Mr. Scott Phillips: https://sourceforge.net/u/thatguy/profile - Script owner
  Unify Communications: https://www.youtube.com/watch?v=wXVLvxrEWeY&t=134s - Video Tutorial
