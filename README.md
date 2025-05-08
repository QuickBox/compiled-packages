# QuickBox Compiled Packages

[![QuickBox](https://img.shields.io/badge/QuickBox-Pro-blueviolet?style=flat-square)](https://quickbox.io)
[![License: MIT](https://img.shields.io/badge/License-MIT-blue.svg?style=flat-square)](https://opensource.org/licenses/MIT)

This repository serves as the central location for **pre-compiled packages** used within the [QuickBox Pro](https://quickbox.io) environment. It contains compiled `.deb` and static binary packages for various open-source applications and supporting libraries, specifically curated and optimized for Debian- and Ubuntu-based systems.

---

## 📦 Purpose

The `compiled-packages` repository exists to:

- Host and organize compiled packages from source for use in QuickBox Pro environments.
- Provide reliable and versioned binaries for tools like **qBittorrent**, **rTorrent**, **Deluge**, **libtorrent**, **Transmission**, and more.
- Serve as a resource for QuickBox users when installing or updating software via the QuickBox package manager and automation scripts.

---

## 📁 Repository Structure

The packages in this repository are organized by distro > arch > and package name, typically as:

```
/<distro>/ 
└── <binary||static>/ 
   └── <package name> 
      └── *.deb 
```


Each package may include:

- `.deb` packages for Debian/Ubuntu systems.
- Static binaries for systems where package managers are not applicable.
- Checksum file `packages.lst` for package integrity verification.

---

## 🛠 Used By

This repository is primarily consumed by:
  
- QuickBox Pro's automated install/update routines  
- Developers and power users compiling or deploying software in headless server environments

---

## 🧰 Example

You might find packages such as:

```bash
bookworm/binary-amd64/rtorrent/rtorrent_0.15.3-1build1_amd64.deb
bullseye/binary-amd64/libtorrent-rasterbar/libtorrent-rasterbar_2.0.11-1build1_amd64.deb
jammy/static-binary/qbittorrent/qbittorrent-nox.qbit5.1.0_lt2.0.11.amd64
```

These are downloaded and installed by QuickBox scripts or manually for custom builds.

---

## 📌 Notes

Packages are compiled to be compatible with Debian 11, 12 and Ubuntu 22.04, depending on the application.

Not all packages are guaranteed to be up to date with upstream releases.

This repository is intended only for use within the QuickBox ecosystem. No support is given directly to this repository.

---

## 📬 Contributing

At this time, contributions are limited to QuickBox maintainers.
If you have suggestions or need a package compiled, please open an issue in the main QuickBox repository:

👉 https://github.com/QuickBox/pro-v3

---

## 📄 License

This repository is licensed under the MIT License.
Binaries are compiled from publicly available open-source projects under their respective licenses.



© 2025 QuickBox.io – All rights reserved.