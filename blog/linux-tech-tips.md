These tips are from my experience with Ubuntu. Other distros may slightly or wildly vary.

- Uninstall Snap
  - First run `snap list`, then `sudo snap remove` them one by one. Takes ages.
  - First remove apps like Firefox, then gnome related ones, then base22 base20 etc, and snapd last.
  - Then `sudo apt remove snapd` to remove snap itself
  - Then `sudo apt-mark hold snapd` so it doesn't reinstall with updates
- Be really careful with do-release-upgrade. If it can break, it will break.
- If you don't see a login screen after boot, gdm probably failed. Press ctrl+alt+F3 to open a console TTY and try fixing from there
  - If that doesn't work, try recovery mode in grub menu and fix from there.
