---
layout: post
title: "Setting Up Ubuntu 24.04 on the Khadas Edge2 (AARCH64)"
date: 2025-10-29
categories: [SBC, Ubuntu, Khadas]
tags: [Khadas Edge2, Ubuntu 24.04, ARM64, SBC, Setup Guide]
author: megatih
description: "A complete guide to installing and configuring Ubuntu 24.04 on the Khadas Edge2 — from system setup to development tools."
---

# Setting Up Ubuntu 24.04 on the Khadas Edge2 (AARCH64)

If you’ve just unboxed a **Khadas Edge2** — congratulations! You’re holding one of the most powerful ARM64 SBCs around, built for AI, edge computing, and even gaming. But before you can unlock its potential, you’ll need a rock-solid Ubuntu 24.04 setup.

This guide walks you through **system-level setup, software installation, and developer tool configuration**, all tested on the **Edge2 running Ubuntu 24.04 (aarch64)**.

---

## 🧩 1. Essential System Setup

Before diving into fancy tools and GUIs, let’s get the essentials right.

### Change the Default Password
Always secure your device first:
```bash
sudo passwd khadas
````

### Update the System

Keep everything fresh and patched:

```bash
sudo apt update && sudo apt upgrade
```

### Remove Preinstalled Bloat (LibreOffice)

Clean up unnecessary packages:

```bash
sudo apt remove --purge 'libreoffice*' && sudo apt autoremove --purge
```

---

## 🧰 2. Core Utilities & System Enhancements

### Install GDebi (GUI Installer for `.deb` Files)

```bash
sudo apt install gdebi
```

### Install Printer Drivers

For Epson or universal printer support:

```bash
sudo apt install printer-driver-escpr
# or for all drivers
sudo apt install printer-driver-all
```

### Install 3D and GPU Utilities

Test your GPU rendering and OpenGL performance:

```bash
sudo apt install mesa-utils mesa-utils-extra glmark2-es2-wayland
```

---

## 🌐 3. Web Browser Installation (Firefox)

Ubuntu 24.04 on ARM doesn’t always ship with Firefox by default, so let’s install the official version from Mozilla.

### Add Mozilla’s APT Repository

```bash
sudo install -d -m 0755 /etc/apt/keyrings
wget -q https://packages.mozilla.org/apt/repo-signing-key.gpg -O- | sudo tee /etc/apt/keyrings/packages.mozilla.org.asc > /dev/null
```

### Verify the Key Fingerprint

```bash
gpg -n -q --import --import-options import-show /etc/apt/keyrings/packages.mozilla.org.asc | awk '/pub/{getline; gsub(/^ +| +$/,""); if($0 == "35BAA0B33E9EB396F59CA838C0BA5CE6DC6315A3") print "\nThe key fingerprint matches ("$0").\n"; else print "\nVerification failed: the fingerprint ("$0") does not match the expected one.\n"}'
```

### Add the Repository Source

For Debian-based Ubuntu 24.04 (“Trixie and newer”):

```bash
cat <<EOF | sudo tee /etc/apt/sources.list.d/mozilla.sources
Types: deb
URIs: https://packages.mozilla.org/apt
Suites: mozilla
Components: main
Signed-By: /etc/apt/keyrings/packages.mozilla.org.asc
EOF
```

### Set Priority for Mozilla Packages

```bash
echo '
Package: *
Pin: origin packages.mozilla.org
Pin-Priority: 1000
' | sudo tee /etc/apt/preferences.d/mozilla
```

### Install Firefox

```bash
sudo apt update && sudo apt install firefox
```

---

## 🖋️ 4. Fonts and Aesthetic Improvements

Make your desktop and IDEs look great:

```bash
sudo apt install fonts-opensymbol fonts-ibm-plex fonts-firacode fonts-jetbrains-mono fonts-jetbrains-mono-web fonts-noto fonts-roboto fonts-font-awesome
```

---

## 💻 5. Developer Environment Setup

### Install BellSoft Liberica JDK 25

A stable Java runtime for ARM64:

```bash
wget -q -O - https://download.bell-sw.com/pki/GPG-KEY-bellsoft | gpg --dearmor | sudo tee /etc/apt/keyrings/GPG-KEY-bellsoft.gpg > /dev/null
echo "deb [arch=$(dpkg --print-architecture) signed-by=/etc/apt/keyrings/GPG-KEY-bellsoft.gpg] https://apt.bell-sw.com/ stable main" | sudo tee /etc/apt/sources.list.d/bellsoft.list
sudo apt update
sudo apt install bellsoft-java25-full
```

### Download Apache Maven

Visit: [https://maven.apache.org/download.cgi](https://maven.apache.org/download.cgi)

### Download Gradle

Visit: [https://gradle.org/next-steps/?version=9.1.0&format=bin](https://gradle.org/next-steps/?version=9.1.0&format=bin)

### Install Go

Visit: [https://go.dev/dl/](https://go.dev/dl/)

### Install Node.js & npm

Visit: [https://nodejs.org/en/download/current](https://nodejs.org/en/download/current)

### Install Miniforge (for Conda & Python)

Visit: [https://github.com/conda-forge/miniforge/releases](https://github.com/conda-forge/miniforge/releases)

---

## 🧠 6. AI and Coding Tools

### Install Qwen Code

Qwen is an open-source code LLM—perfect for local coding assistance:
[https://github.com/QwenLM/qwen-code](https://github.com/QwenLM/qwen-code)

### Install Visual Studio Code

ARM64 build available at:
[https://code.visualstudio.com/Download](https://code.visualstudio.com/Download)

---

## 🎮 7. Graphics & Game Development

### Install Raylib (C/C++ Game Framework)

```bash
sudo add-apt-repository ppa:texus/raylib
sudo apt update
sudo apt install libraylib-dev
```

---

## 🧾 8. Office & Productivity

### Download LibreOffice (ARM64 Build)

Visit: [https://www.libreoffice.org/download/download-libreoffice/?type=deb-aarch64&version=25.8.2&lang=en-US](https://www.libreoffice.org/download/download-libreoffice/?type=deb-aarch64&version=25.8.2&lang=en-US)

---

## 🚀 Final Thoughts

Once you’ve completed these steps, your **Khadas Edge2** will be transformed into a fully capable ARM64 workstation — ready for development, AI research, or multimedia workloads.

The combination of **Ubuntu 24.04** and the **RK3588 SoC** provides blazing performance while staying efficient and compact.

Happy hacking on the Edge2! 🧑‍💻🔥

---

**Did you find this guide helpful?**
Leave a comment below or share your own setup tips with the Khadas community!
