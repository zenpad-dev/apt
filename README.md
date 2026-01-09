# Zenpad APT Repository

Official APT repository for [Zenpad](https://zenpad-dev.github.io) - A lightweight, keyboard-driven text editor for Linux.

## Installation

### Quick Install (Recommended)

```bash
# Add GPG key
curl -fsSL https://zenpad-dev.github.io/apt/zenpad.gpg | sudo gpg --dearmor -o /usr/share/keyrings/zenpad.gpg

# Add repository
echo "deb [signed-by=/usr/share/keyrings/zenpad.gpg] https://zenpad-dev.github.io/apt stable main" | sudo tee /etc/apt/sources.list.d/zenpad.list

# Install
sudo apt update
sudo apt install zenpad
```

### Updates

```bash
sudo apt update && sudo apt upgrade zenpad
```

### Remove

```bash
sudo apt remove zenpad
sudo rm /etc/apt/sources.list.d/zenpad.list /usr/share/keyrings/zenpad.gpg
```

## Available Packages

| Package | Version | Architecture |
|---------|---------|--------------|
| zenpad  | 1.3.0   | all          |

## Repository Structure

```
├── dists/stable/main/binary-amd64/
│   ├── Packages, Packages.gz
│   ├── Release, Release.gpg, InRelease
└── pool/main/z/zenpad/
    └── zenpad_*.deb
```

## Links

- [Website](https://zenpad-dev.github.io)
- [Source Code](https://github.com/jagdishtripathy/zenpad)
- [Releases](https://github.com/jagdishtripathy/zenpad/releases)

---
Maintained by [Zenpad Team](https://github.com/zenpad-dev)
