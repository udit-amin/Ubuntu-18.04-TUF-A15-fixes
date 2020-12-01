On fresh install, wifi is disabled on many devices for Ubuntu 18.04.

For the Asus TUF A15, Ubuntu 18.04 comes with firmware 1.173. Updating it to 1.187.6 fixes this issue. To do so 

1) Check the firmware Ubuntu is currently on: 

       apt list | grep linux-firmware

2) Update the firmware
      
       sudo apt update
       wget http://mirrors.kernel.org/ubuntu/pool/main/l/linux-firmware/linux-firmware_1.187.2_all.deb
       sudo dpkg -i linux-firmware_1.187.2_all.deb

3) Reboot the system
       
       sudo reboot

