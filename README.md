# archlinux-settings
* install arch linux using the guide in arch wiki
  * for dual boot I recommand this tutorial: https://www.youtube.com/watch?v=C3D_qzw94v8

## netwrok issue
* install dhcpcd (using archoiso)
* run `ip link` and copy the port name (mine was enp2s0)
* run `systemctl enable dhcpcd@enp2s0` and `systemctl start dhcpcd@enp2s0`

## basics
* instsall sudo: `pacman -S sudo`
* install vim: `pacman -S vim`
* install firefox
