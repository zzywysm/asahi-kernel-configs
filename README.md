# asahi-kernel-configs

Useful if you want to build your own Asahi Linux kernel for Apple Silicon.

~WARNING: These configs are not compatible with the dracut configuration provided by the Asahi Linux team, as the official Asahi Linux distros build most of their drivers as modules, whereas we move many Asahi drivers into the kernel image.~  As of https://github.com/AsahiLinux/asahi-scripts/commit/4acd310cd8c394f9ec2e7e7506d89b7bb3c3ca39 I don't think this is an issue anymore.

Current kernel configurations:

**asahi-kernel-6.8-gentoo-comprehensive**: Intended to provide distkernel-level support for Asahi on Gentoo, via chadmed's `asahi-overlay` project.  Should work on any arm64 distro to provide support for most (if not all) things you could currently plug into an Apple Silicon Mac (and that are supported by vanilla Linux).

https://github.com/chadmed/asahi-overlay

**asahi-kernel-6.8-nixos-barebones**: My production kernel on my MacBook Air running NixOS. This config is missing a lot of drivers, including Bluetooth.  The goal here is to make a very tiny kernel that still works as a daily driver, but don't expect uncommon/rare peripherals to work.

https://github.com/zzywysm/nixos-asahi
