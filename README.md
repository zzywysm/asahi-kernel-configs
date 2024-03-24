# asahi-kernel-configs

Useful if you want to build your own Asahi Linux kernel for Apple Silicon.

WARNING: These configs are not compatible with the dracut configuration provided by the Asahi Linux team, as the official Asahi Linux distros build most of their drivers as modules, whereas we move many Asahi drivers into the kernel image.

Current kernel configurations:

**asahi-kernel-6.6-gentoo-comprehensive**: Intended to provide distkernel-level support for Asahi on Gentoo, via chadmed's `asahi-overlay` project.

https://github.com/chadmed/asahi-overlay

**asahi-kernel-6.6-nixos-barebones**: My production kernel on my MacBook Air running NixOS. Is missing a lot of drivers, including Bluetooth.

https://github.com/zzywysm/nixos-asahi
