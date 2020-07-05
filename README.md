# PSL8_usbSERVICE
## USB script to detect, mount and unmount a usb

> STEPS:

- first of all copy and clone the git project in your terminal.

  - `git clone https://github.com/zahrah925/PSL8_usbSERVICE.git`
  
- Insert your USB and run the script.

  - `./usbDetectServ`


## Create a service with the script

> STEPS:

- Create the service.

  - `sudo nano /etc/systemd/system/daemon.service`

- Write the following codes in the daemon.service
  - Edit the User and the ExecStart to your own username and path.
  
  ![alt text](/home/zahrah/Pictures/Screenshot from 2020-07-05 15-35-28.png)

- Save and exit the nano.


-  Type the following commands to execute the service.

  - `systemctl start daemon`
  
  - `systemctl enable daemon`
  
  - `systemctl status daemon.service`

- To stop and delete the service:

  - `systemctl stop daemon.service`
  
  - `sudo systemctl disable daemon.service`
  
  - `sudo rm daemon.service`
  
  

