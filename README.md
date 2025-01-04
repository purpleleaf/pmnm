# pmnm
Poor man network manager

A simple network manager for Arch Linux based distro that glues some bash with some other lightweight tools (ifplugd, busybox, tint2 executor, etc)

It is mainly targeted to Artix Linux and Obarun but any Linux distro providing the required dependencies should be able to run it.

At the moment only automatic configuration trough dhcp or manual settings through /etc/network/interfaces file are provided.
You can use your preferred wi-fi configuration tool (wicd, wpa_supplicant).
Ifplugd will monitor if a  eth connection is present; on artix and obarun if a wifi connection is active, its metric is set to a lower value then the  eth  network metric, so be advised that if both  eth and wifi are active, eth will have priority.

To install clone this repo and  copy all files to the corresponding position on your filesystem. Install busybox udhcpc and ifup symlinks.

A tint2 executors that monitors if network is reached by wired or wireless connection is provided by my [pmt2e respository](https://github.com/purpleleaf/pmt2e).

Dependencies: ifplugd, busybox, wicd | wpa_supplicant
