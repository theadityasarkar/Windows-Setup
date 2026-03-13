# Windows Setup Guide: Essential Apps and Tools for Fresh Install

A comprehensive, tested guide for setting up a fresh Windows 11 machine with essential software, productivity tools, and system optimization utilities. Every tool listed here has been personally verified and is actively used on production systems.

## Who This Guide Is For

This guide is designed for:
- Users performing a fresh Windows 11 installation
- System administrators setting up multiple machines
- Developers configuring new workstations
- Power users optimizing Windows performance
- Anyone wanting a curated list of reliable Windows software

## What This Setup Helps You Achieve

By following this guide, you will:
- Install essential productivity and development tools
- Optimize Windows 11 performance and remove bloatware
- Set up download managers and media players
- Configure system utilities for maintenance and monitoring
- Activate Windows and Office (using official Microsoft Activation Scripts)
- Secure your network with VPN solutions

## Prerequisites

Before starting:
- Fresh Windows 11 installation or administrator access to Windows 11
- Active internet connection
- Administrator privileges on your machine
- Basic familiarity with PowerShell (all commands are copy-paste ready)

## Table of Contents

- [Quick Start](#quick-start)
- [Windows 11](#windows-11)
- [Microsoft Office 365](#microsoft-office-365)
- [Windows Utility by Chris Titus Tech](#windows-utility-by-chris-titus-tech)
- [Browsers](#browsers)
- [Warp VPN by Cloudflare](#warp-vpn-by-cloudflare)
- [qBittorrent](#qbittorrent)
- [Internet Download Manager (IDM)](#internet-download-manager-idm)
- [WinRAR](#winrar)
- [System Utilities](#system-utilities)
- [Spotify (Ad-Free with SpotX)](#spotify-ad-free-with-spotx)
- [VLC Media Player](#vlc-media-player)
- [Visual Studio Code](#visual-studio-code)
- [NVIDIA App](#nvidia-app)
- [MSI Afterburner](#msi-afterburner)
- [How to Run PowerShell Scripts](#how-to-run-powershell-scripts)
- [Troubleshooting](#troubleshooting)
- [Frequently Asked Questions](#frequently-asked-questions)
- [Credits](#credits)

## Quick Start

**IMPORTANT:** All PowerShell scripts must be run as Administrator.

To open PowerShell as Administrator:
1. Right-click the Windows Start menu (or press `Win + X`)
2. Select "Terminal (Admin)" or "PowerShell (Admin)"
3. Click "Yes" when prompted for permission

## Windows 11

The latest operating system by Microsoft with modern design, improved performance, and enhanced security features.

| Resource | Link |
|----------|------|
| Official Download | [Download Windows 11](https://www.microsoft.com/en-us/software-download/windows11) |

**Windows Activation Script**

Activate Windows 11 to unlock all features and remove watermark using the Microsoft Activation Scripts project:

```powershell
irm https://get.activated.win | iex
```

## Microsoft Office 365

Essential office suite including Word, Excel, PowerPoint, Outlook, and more. Required for professional and academic work.

| Resource | Link |
|----------|------|
| Official Download | [Download Office 365](https://www.microsoft.com/en-us/microsoft-365/download-office#download) |

**Office Activation Script**

Activate Office 365 to unlock full features:

```powershell
irm https://get.activated.win | iex
```

## Windows Utility by Chris Titus Tech

An all-in-one tool for debloating Windows, optimizing performance, applying privacy tweaks, and installing common software with one click.

```powershell
iwr -useb https://christitus.com/win | iex
```

## Browsers

### Brave Browser (Recommended)

Privacy-focused browser with built-in ad blocking and tracker protection. Faster browsing with reduced data usage.

| Resource | Link |
|----------|------|
| Official Download | [Download Brave](https://brave.com/download/) |

**Why Brave?** Built-in ad blocker and privacy features without requiring extensions.

### Google Chrome

The most popular browser by Google. Fast, syncs with Google account, and supports thousands of extensions.

| Resource | Link |
|----------|------|
| Official Download | [Download Chrome](https://www.google.com/chrome/what-you-make-of-it/) |

## Warp VPN by Cloudflare

Free VPN service by Cloudflare that encrypts internet connection and protects privacy. Fast, reliable, and privacy-focused.

| Resource | Link |
|----------|------|
| Download | [Download Warp VPN](https://filecr.com/windows/warp-vpn-by-cloudflare/) |

## qBittorrent

Free and open-source torrent client with no ads. Efficient for downloading large files through BitTorrent protocol.

| Resource | Link |
|----------|------|
| Official Download | [Download qBittorrent](https://www.qbittorrent.org/download) |

## Internet Download Manager (IDM)

Accelerates downloads by up to 5x, supports pause/resume, download scheduling, and video grabbing from websites.

| Resource | Link |
|----------|------|
| Official Download | [Download IDM](https://www.internetdownloadmanager.com/download.html) |

**IDM Activation Script**

```powershell
irm https://coporton.com/ias | iex
```

## WinRAR

File compression and extraction tool supporting ZIP, RAR, 7Z, and other archive formats.

| Resource | Link |
|----------|------|
| Official Download | [Download WinRAR](https://www.rarlab.com/download.htm) |

**WinRAR Activation Script**

```powershell
irm https://naeembolchhi.github.io/WinRAR-Activator/WRA.ps1 | iex
```

## System Utilities

### Driver Booster

Automatically finds and updates outdated drivers with one click. Drivers enable hardware components to communicate with Windows.

| Resource | Link |
|----------|------|
| Official Download | [Download Driver Booster](https://www.iobit.com/en/driver-booster.php) |
| Free License | [Get License Key](https://techno360.in/driver-booster-13-pro-free-license/) |

### IObit Uninstaller

Completely removes programs along with leftover files and registry entries. More thorough than Windows built-in uninstaller.

| Resource | Link |
|----------|------|
| Official Download | [Download IObit Uninstaller](https://www.iobit.com/en/advanceduninstaller.php) |
| Free License | [Get License Key](https://techno360.in/iobit-uninstaller-15-pro-free-license/) |

### Advanced SystemCare

All-in-one PC optimization tool that cleans junk files, fixes registry errors, and improves system performance.

| Resource | Link |
|----------|------|
| Official Download | [Download Advanced SystemCare](https://www.iobit.com/en/advancedsystemcarefree.php) |
| Free License | [Get License Key](https://techno360.in/advanced-systemcare-19-pro-free-license/) |

### Microsoft PowerToys

Official Microsoft utilities that enhance Windows productivity. Includes FancyZones (window layouts), PowerRename (bulk rename), Color Picker, Image Resizer, and more.

| Resource | Link |
|----------|------|
| Official Download | [Download PowerToys](https://learn.microsoft.com/en-us/windows/powertoys/) |

## Spotify (Ad-Free with SpotX)

World's most popular music streaming service. SpotX modification removes ads from the free version.

| Resource | Link |
|----------|------|
| Official Download | [Download Spotify](https://www.spotify.com/download/windows/) |

**SpotX Ad-Free Script**

Run after installing Spotify:

```powershell
iex "& { $(iwr -useb 'https://raw.githubusercontent.com/SpotX-Official/SpotX/refs/heads/main/run.ps1') } -new_theme"
```

## VLC Media Player

Universal media player that plays virtually any audio or video format without additional codecs.

| Resource | Link |
|----------|------|
| Official Download | [Download VLC](https://www.videolan.org/vlc/download-windows.html) |

## Visual Studio Code

Free, lightweight code editor by Microsoft. Supports all programming languages with thousands of extensions, built-in Git support, and intelligent code completion.

| Resource | Link |
|----------|------|
| Official Download | [Download VS Code](https://code.visualstudio.com/download) |

## NVIDIA App

Official NVIDIA application for managing graphics cards. Updates GPU drivers, optimizes game settings, and enables gameplay recording.

**Note:** Only install if you have an NVIDIA graphics card. Check by pressing `Win + X` → Device Manager → Display adapters.

| Resource | Link |
|----------|------|
| Official Download | [Download NVIDIA App](https://www.nvidia.com/en-in/software/nvidia-app/) |

## MSI Afterburner

Real-time system monitoring tool that displays FPS, GPU temperature, CPU usage, and RAM usage as an on-screen overlay. Also supports graphics card overclocking.

Recommended for users who want to monitor PC performance during gaming or stress testing.

| Resource | Link |
|----------|------|
| Official Download | [Download MSI Afterburner](https://www.msi.com/Landing/afterburner/graphics-cards) |

## How to Run PowerShell Scripts

### Step 1: Open PowerShell as Administrator

1. Right-click the Windows Start menu (or press `Win + X`)
2. Select "Terminal (Admin)" or "PowerShell (Admin)"
3. Click "Yes" when asked for permission

### Step 2: Copy and Execute Script

1. Triple-click the script command to select the entire line
2. Copy with `Ctrl + C`
3. Right-click in PowerShell window to paste
4. Press Enter to execute

## Troubleshooting

| Issue | Solution |
|-------|----------|
| Script not running | Verify PowerShell is opened as Administrator |
| Execution policy error | Run `Set-ExecutionPolicy Bypass -Scope Process`, then retry script |
| Download blocked by antivirus | Temporarily disable antivirus or add exception |
| Connection error | Verify internet connection and retry |
| Command not found error | Ensure entire command was copied correctly |

## Frequently Asked Questions

### Are these activation scripts safe?

Yes. All activation scripts referenced in this guide are from well-established open-source projects with thousands of users and active maintenance. The Microsoft Activation Scripts project, for example, uses official Microsoft KMS servers.

### Do I need to install everything listed?

No. This is a curated collection of tools. Install only what you need based on your use case. The Essential System Tools and System Utilities sections are recommended for all users.

### Will these scripts work on Windows 10?

Most scripts and applications support both Windows 10 and Windows 11. However, this guide is optimized for Windows 11 fresh installations.

### How often should I update drivers?

Use Driver Booster monthly or when experiencing hardware issues. Graphics card drivers should be updated more frequently if you game regularly.

### Can I use these scripts on multiple computers?

Yes. All scripts can be run on multiple machines. Some activation scripts are designed specifically for multi-machine deployments.

### What if a script fails?

Check the Troubleshooting section first. If issues persist, visit the original project repository (linked in Credits section) for support.

### Are there alternatives to the recommended software?

Yes. This guide focuses on tested, reliable options. Alternatives exist for most categories but may require separate research.

## Credits

| Contributor | Project |
|-------------|---------|
| [@iitzz-aadii](https://github.com/iitzz-aadii) | Repository maintainer |
| [Microsoft Activation Scripts](https://github.com/massgravel/Microsoft-Activation-Scripts) | Windows and Office activation |
| [Chris Titus Tech](https://github.com/ChrisTitusTech/winutil) | Windows Utility tool |
| [SpotX](https://github.com/SpotX-Official/SpotX) | Spotify ad-free modification |
| [IDM Activation Script](https://github.com/lstprjct/IDM-Activation-Script) | IDM activation |
| [WinRAR Activator](https://github.com/naeembolchhi/WinRAR-Activator) | WinRAR activation |

## Disclaimer

This repository is for educational purposes. Always download software from official sources when possible. The maintainers are not responsible for any misuse of the scripts or tools provided here.

## License

This project is open source and available for anyone to use, modify, and distribute.

---

**Found this helpful?** Star this repository to support the project and help others discover this guide.
