# Arch-TUI-Installer

Arch-TUI-Installer is an Installer for [Archlinux](https://archlinux.org).

It's based on the [Arch Basic Install](https://gitlab.com/sontypiminternet/arch-basic)-Repository on GitLab.

[![GitHub release (latest by date)](https://img.shields.io/github/v/release/Niklas20114552/arch-tui-installer?display_name=tag&label=Release&style=flat-square)](https://github.com/Niklas20114552/arch-tui-installer/releases/latest)
[![Website](https://img.shields.io/static/v1?label=Website&message=click&color=blue&style=flat-square)](https://arch-tui-installer.github.io)
[![Isomaker](https://img.shields.io/static/v1?label=Isomaker&message=click&color=blue&style=flat-square)](https://github.com/arch-tui-installer/arch-tui-installer-isomaker)

# I need your help!

You can download both ```lang.conf``` (there is also one in the ```installed``` folder) files and make a translation.

When you're done, please submit it via the Issue-Tab, with the Title:

Translation: [YOUR-LANGUAGE]

## Troubleshooting

### UEFI with QEMU:

When you are having troubles booting the ISO:
Please use the `UEFI x86_64: /usr/share/OVMF/OVMF_CODE_4M.fd` Firmware, not `UEFI`
## Installation with the ISO-File

In the [Releases](https://github.com/Niklas20114552/arch-tui-installer/releases) Tab download the latest ISO File. Then attach the ISO to the VM, burn it to a DVD or copy it to an USB-Stick.
Then type this into the Terminal:

```bash
setup
```
## Manual Installation
### Recommended when key errors occur. (such as Invalid or broken Package (PGP-Signature)
Download the [Archlinux ISO](https://archlinux.org/download/)

In Terminal type this:
```bash
pacman --needed --noconfirm -Sy dialog git
curl -O https://raw.githubusercontent.com/Niklas20114552/arch-tui-installer/main/updater
chmod +x updater
./updater
```

## I found an Issue!

Thank you! Please enable the debug-mode:

Normal installation: Run setup with `setup --debug`

Manual installation: Run setup with `setup --debug`, after you have started the Updater

Than look for error-messages and write it down. Please report the error in the [Issue](https://github.com/Niklas20114552/arch-tui-installer/issues)-Tab. But first check if it has already been reported
