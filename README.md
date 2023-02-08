# mount_reminder
Systemd service to remind me to mount filesystems which have been unmounted from reboot, etc.

## Install
1. Copy files under `fs` into place.
2. `sudo systemctl enable --now $(systemd-escape --template mountreminder@.service "/path/to/mount/point")`
