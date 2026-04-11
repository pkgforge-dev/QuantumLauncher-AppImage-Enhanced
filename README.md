<div align="center">

# QuantumLauncher-AppImage-Enhanced 🐧

[![GitHub Downloads](https://img.shields.io/github/downloads/pkgforge-dev/QuantumLauncher-AppImage-Enhanced/total?logo=github&label=GitHub%20Downloads)](https://github.com/pkgforge-dev/QuantumLauncher-AppImage-Enhanced/releases/latest)
[![CI Build Status](https://github.com/pkgforge-dev/QuantumLauncher-AppImage-Enhanced/actions/workflows/appimage.yml/badge.svg)](https://github.com/pkgforge-dev/QuantumLauncher-AppImage-Enhanced/releases/latest)
[![Latest Stable Release](https://img.shields.io/github/v/release/pkgforge-dev/QuantumLauncher-AppImage-Enhanced)](https://github.com/pkgforge-dev/QuantumLauncher-AppImage-Enhanced/releases/latest)

<p align="center">
  <img src="https://github.com/Mrmayman/quantumlauncher/blob/main/assets/icon/128x128/ql_logo.png" width="128" />
</p>

Improved AppImage **independent of the host libc** which makes able to work on very very old distros as well as musl-libc distros like alpine linux.
Most minecraft launchers just download java in the user's home and do not take into consideration that downloaded java may not be able to work on the host system at all, due to the `java` binaries being dynamic and depending on the glibc dynamic linker in `/lib64`. **This AppImages fixes that issue by intercepting the `execve` calls to the user's `java` to run with sharun which allows using a portable dynamic linker instead.**

| Latest Stable Release | Upstream URL |
| :---: | :---: |
| [Click here](https://github.com/pkgforge-dev/QuantumLauncher-AppImage-Enhanced/releases/latest) | [Click here](https://github.com/Mrmayman/quantumlauncher) |

</div>

---

AppImage made using [sharun](https://github.com/VHSgunzo/sharun) and its wrapper [quick-sharun](https://github.com/pkgforge-dev/Anylinux-AppImages/blob/main/useful-tools/quick-sharun.sh), which makes it extremely easy to turn any binary into a portable package reliably without using containers or similar tricks. 

**This AppImage bundles everything and it should work on any Linux distro, including old and musl-based ones.**

This AppImage doesn't require FUSE to run at all, thanks to the [uruntime](https://github.com/VHSgunzo/uruntime).

This AppImage is also supplied with a self-updater by default, so any updates to this application won't be missed, you will be prompted for permission to check for updates and if agreed you will then be notified when a new update is available.

Self-updater is disabled by default if AppImage managers like [am](https://github.com/ivan-hc/AM), [soar](https://github.com/pkgforge/soar) or [dbin](https://github.com/xplshn/dbin) exist, which manage AppImage updates.

<details>
  <summary><b><i>raison d'être</i></b></summary>
    <img src="https://github.com/user-attachments/assets/d40067a6-37d2-4784-927c-2c7f7cc6104b" alt="Inspiration Image">
  </a>
</details>

---

More at: [AnyLinux-AppImages](https://pkgforge-dev.github.io/Anylinux-AppImages/)
