# archlinux-settings
* install arch linux using the guide in arch wiki
  * for dual boot I recommand this tutorial: https://www.youtube.com/watch?v=C3D_qzw94v8

## netwrok issue (in lenovo z51-70)
* install dhcpcd (using archoiso)
* run `ip link` and copy the port name (mine was enp2s0)
* run `systemctl enable dhcpcd@enp2s0` and `systemctl start dhcpcd@enp2s0`

## basics
### install basic DE utilities:
* https://github.com/LukeSmithxyz/LARBS
#### change browser (optional)
larbs comes by default with `brave` browser. you can change it by:
1. installing chromium/firefox
2. uninstalling brave
3. change default `BROWSER` env var in `~/.zprofile` file


### instsall hebrew:
(see "Generating locales" section at https://wiki.archlinux.org/index.php/Locale)
* uncomment `he_IL.UTF-8 UTF-8` in `/etc/locale.gen`
* run `locale-gen`
* add `setxkbmap -option grp:switch,grp:alt_shift_toggle, us,il` in your ~/.xprofile (or initrc) file
