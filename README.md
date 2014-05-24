System daemon for reading info about GPU clocks and volts and pass this data to [radeon-profile](https://github.com/marazmista/radeon-profile) so the GUI application can be run as normal user.

Supprts only open source xf86-video-ati driver.

# Bulid

Type: `qmake-qt4 && make` in source directory.

# systemd service

There is a service file for systemd in radeon-profile-daemon/extra. If installed manually, copy service file to `/etc/systemd/system/`. After that, execute `systemctl enable radeon-profile-daemon.service` and `systemctl start radeon-profile-daemon.service` to make the daemon running.
