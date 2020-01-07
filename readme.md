ID-OS
=====

An *experimental* operating system for decentralized apps.
Based on [Balena OS][1].

Installation
------------

ID-OS is currently only tested on a Raspberry Pi 4 with 4Gb. Follow these steps
to install ID-OS:

  1. Download the [Balena OS development image][2] for Raspberry Pi 4.
  2. Flash the image to an SD card for your Pi. You can use [Balena Etcher][3]
      for this.
  3. Install the [Balena CLI][4] on the development machine where you checked
      out this repository.
  4. Connect the Pi to the same network as your development machine using an
      ethernet cable. A WiFi connection can be configured later, but for now
      you'll need a fixed connection to the Pi.
  5. Power up the Pi. It should become visible in the network as the
      'balena.local' host.
  6. Invoke `balena push balena.local` in the root of this project. This will
      push the docker configuration from this repository to the Pi.

WiFi Setup
----------

ID-OS includes the [Wifi-Connect][5] software from Balena. This means that the
Pi exposes an access point called 'Wifi Connect'. You can connect to this access
point using a mobile device, which will pop-up a dialog for configuring the WiFi
connection of ID-OS.


[1]: https://balena.io
[2]: https://www.balena.io/os/#download
[3]: https://www.balena.io/etcher/
[4]: https://github.com/balena-io/balena-cli/blob/master/INSTALL.md
[5]: https://github.com/balena-io/wifi-connect
