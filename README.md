# pmnm
Poor man network manager

A simple network manager that glues with some bash some other lightweight tools (iw, jgmenu, busybox, tint2 executor, etc)

It is mainly targeted to Artix Linux and Obarun but any Linux distro providing the required dependencies should be able to run it.

At the moment only automatic configuration trough dhcp and manual settings trhough /etc/interfaces file modification are provided, with a tint2 executors that monitors if network is reached by wired or wireless connection.

To use the tint2 executor simply create an executor on tint2 setting manager and use pmna as Command with a 2 second Interval and Show icon flag on.

