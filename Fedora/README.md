# Tested on the following hardware:

- darp9 (Open Firmware)

## Features

- [ ] Firmware Updates (CLI and GUI)
- [ ] Keyboard backlight key combo(s)
- [ ] Screen backlight key combos
- [ ] Sound key combos
- [ ] System76 Driver Log creation
- [ ] Graphic Switching
- [ ] Power profiles 

| Item | Notes | Grade |
|:--------:|:------------:|:----:|
| Booting from media | Boots up to the installer with no changes | A |
| OS Install | OS installs to the drive with no changes |  |
| Booting from new install | OS boots from the drive with no changes | |
| Install System76 Software | Software is available from the 3rd Party Repo | |
| System76 Software | Only software that does not work is system76-power GNOME Extension with GNOME 44 | |

For System76 Power you do need to mask power-profiles-daemon:

```bash
sudo systemctl mask power-profiles-daemon.service
```

 GNOME Shell Extension does not support GNOME 44
