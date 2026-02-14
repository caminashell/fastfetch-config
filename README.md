# Fastfetch Configuration

![2026-02-14](https://github.com/user-attachments/assets/841fc849-b4ff-47fc-8297-74486d7271ef)

> Fastfetch is a [neofetch](https://github.com/dylanaraps/neofetch)-like tool for fetching system information and displaying it prettily. It is written mainly in C, with performance and customizability in mind. Currently, Linux, Android, FreeBSD, macOS, SunOS and Windows 7+ are supported.

[![GitHub Workflow Status (with event)](https://img.shields.io/github/actions/workflow/status/fastfetch-cli/fastfetch/ci.yml)](https://github.com/fastfetch-cli/fastfetch/actions)
[![GitHub license](https://img.shields.io/github/license/fastfetch-cli/fastfetch)](https://github.com/fastfetch-cli/fastfetch/blob/dev/LICENSE)
[![GitHub contributors](https://img.shields.io/github/contributors/fastfetch-cli/fastfetch)](https://github.com/fastfetch-cli/fastfetch/graphs/contributors)
[![GitHub top language](https://img.shields.io/github/languages/top/fastfetch-cli/fastfetch?logo=c&label=)](https://github.com/fastfetch-cli/fastfetch/blob/dev/CMakeLists.txt#L5)
[![GitHub commit activity (branch)](https://img.shields.io/github/commit-activity/m/fastfetch-cli/fastfetch)](https://github.com/fastfetch-cli/fastfetch/commits)  
[![homebrew downloads](https://img.shields.io/homebrew/installs/dm/fastfetch?logo=homebrew)](https://formulae.brew.sh/formula/fastfetch#default)
[![GitHub all releases](https://img.shields.io/github/downloads/fastfetch-cli/fastfetch/total?logo=github)](https://github.com/fastfetch-cli/fastfetch/releases)  
[![GitHub release (with filter)](https://img.shields.io/github/v/release/fastfetch-cli/fastfetch?logo=github)](https://github.com/fastfetch-cli/fastfetch/releases)
[![latest packaged version(s)](https://repology.org/badge/latest-versions/fastfetch.svg)](https://repology.org/project/fastfetch/versions)
[![Packaging status](https://repology.org/badge/tiny-repos/fastfetch.svg)](https://repology.org/project/fastfetch/versions)

To install Fastfetch, please consult [the official repository](https://github.com/fastfetch-cli/fastfetch).

## Config Installation

To use this configuration, install the `config.jsonc` file to `~/.config/fastfetch/`

If you do not have this folder, create it:

```sh
$ mkdir -p ~/.config/fastfetch
```

Create the file with your editor (Nano, Vim, etc.), or create the file in the command line:

```sh
$ touch ~/.config/fastfetch/config.jsonc
```

Copy the entire contents of the `config.json` file from this repository to your newly created file.

Save and exit the file.

Run `fastfetch` within your terminal.

## What the configuration shows

### Software

- Operating system release
- Kernel version
- System service manager version
- Installed packages
- Shell type
- Terminal version
- Terminal font
- Display environment
- Window manager
- Login manager
- Window manager theme
- Desktop environment theme
- Desktop icons theme
- OpenGL version
- Vulkan version
- Locale

### Hardware

- Host mainboard identifier
- BIOS/UEFI release version
- CPU type
- GPU type
- Memory currently in use
- Swap file in use
- Disk information
  - Showing `btrfs` module.
  - Replace `btrfs` module with `disk` or `physicaldisk` if not using BTRFS.
- Display monitor
- Screen resolution information
- Brightness detail _(if applicable)_
- Battery detail _(if applicable)_
- Power detail _(if applicable)_
- Audio device currently in use
- Bluetooth devices

### Time Information

- Age: Time since OS installation
- Uptime: Since boot
- Local date & time information, including week & day in the year.

### Misc.

- OS logo right-aligned
- Terminal colours at foot

> [!TIP]
> Add the following alias to your `.bashrc` or `.zshrc` file as a quick-key shortcut.
> ```sh
> alias ff="fastfetch"
> ```
