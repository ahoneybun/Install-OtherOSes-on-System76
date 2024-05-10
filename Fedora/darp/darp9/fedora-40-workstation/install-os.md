# ISO Tested

ISO filename: Fedora-Workstation-Live-x86_64-40-1.14.iso

## Features

- [ ] Firmware Updates (CLI and GUI)
- [x] Keyboard backlight key combo(s) (works without system76 driver)
- [x] Screen backlight key combos (works without system76 driver)
- [x] Sound key combos (works without system76 driver)
- [ ] System76 Driver Log creation
- [ ] Graphic Switching
- [ ] Power profiles 

| Item | Notes | Grade |
|:--------:|:------------:|:----:|
| Booting from media | Boots up to the installer with no changes | A |
| OS Install | OS installs to the drive with no changes | A |
| Booting from new install | OS boots from the drive with no changes | A |
| Install System76 Software | Software is available from the 3rd Party Repo | |
| System76 Software | Only software that does not work is system76-power GNOME Extension with GNOME 44 | |

For System76 Power you do need to mask power-profiles-daemon:

```bash
sudo systemctl mask power-profiles-daemon.service
```

 GNOME Shell Extension does not support GNOME 44
