# OpenWrt packages feed
[![FOSSA Status](https://app.fossa.io/api/projects/git%2Bgithub.com%2Fjs3725831%2Fpackages.svg?type=shield)](https://app.fossa.io/projects/git%2Bgithub.com%2Fjs3725831%2Fpackages?ref=badge_shield)


## Description

This is the OpenWrt "packages"-feed containing community-maintained build scripts, options and patches for applications, modules and libraries used within OpenWrt.

Installation of pre-built packages is handled directly by the **opkg** utility within your running OpenWrt system or by using the [OpenWrt SDK](https://openwrt.org/docs/guide-developer/obtain.firmware.sdk) on a build system.

## Usage

This repository is intended to be layered on-top of an OpenWrt buildroot. If you do not have an OpenWrt buildroot installed, see the documentation at: [OpenWrt Buildroot – Installation](https://openwrt.org/docs/guide-developer/build-system/install-buildsystem) on the OpenWrt support site.

This feed is enabled by default. To install all its package definitions, run:
```
./scripts/feeds update packages
./scripts/feeds install -a -p packages
```

## License

See [LICENSE](LICENSE) file.
 

[![FOSSA Status](https://app.fossa.io/api/projects/git%2Bgithub.com%2Fjs3725831%2Fpackages.svg?type=large)](https://app.fossa.io/projects/git%2Bgithub.com%2Fjs3725831%2Fpackages?ref=badge_large)

## Package Guidelines

See [CONTRIBUTING.md](CONTRIBUTING.md) file.