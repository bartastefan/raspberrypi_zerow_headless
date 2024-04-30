When I install a new OS to the SD card via Raspberry Pi Imager, I cannot connect to my Raspberry Pi Zero W, even I set the network connection and the SSH.
This solution solve me the problem.
Create the image to the SD card with the Imager, then copy these 2 files into the Boot.
The SSH is intentionally empty, the Raspbian will be apply the authentication from wpa_supplicant.conf file during the first boot.
The first boot is longer, but eventually the Raspberry pi showing on your network, then you'll able to connect it via SSH.
