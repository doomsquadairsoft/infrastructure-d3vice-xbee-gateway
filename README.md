# infrastructure-d3vice-xbee-gateway
Infrastructure as code - provisioning strategies for https://github.com/doomsquadairsoft/d3vice-xbee-gateway

## Provision a Raspberry Pi Zero

First of all, you gotta use some software on your dev machine to flash the SD card that the Raspberry Pi Zero will use.

### Dependencies

  * [Hypriot Flash](https://github.com/hypriot/flash/releases) which is used to flash HypriotOS onto the RPi's SD card.
  * [cloud-init file](https://cloudinit.readthedocs.io/en/18.5/topics/examples.html) which is used to configure the RPi.

### Flash HypriotOS onto the SD Card

We can use Hypriot's flash utility for this, which can pull the hypriotOS image directly from GitHub. Just check the [HypriotOS releases page](https://github.com/hypriot/image-builder-rpi/releases) to make sure you're getting the most up-to-date version.

    flash --hostname node01 https://github.com/hypriot/image-builder-rpi/releases/download/v1.10.0/hypriotos-rpi-v1.10.0.img.zip


 

