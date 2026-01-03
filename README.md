<div align="center">

[English](README.md) | [简体中文](README.zh-CN.md)

</div>


<p align="center">
  <img src="assets/Logo-Default.png" alt="ClashMac Logo" width="300" style="filter: drop-shadow(0 4px 12px rgba(0, 0, 0, 0.15));">
</p>
<h1 align="center">ClashMac</h1>
<h3 align="center" style="margin-top: 0; margin-bottom: 10px;">Lightweight macOS Clash Menu Bar Client</h3>
<p align="center">
  🌐 <a href="https://clashmac.app"><strong>Official Website: clashmac.app</strong></a>
</p>

<p align="center" style="margin-top: 0; margin-bottom: 20px;">
  <a href="https://github.com/666OS/ClashMac/releases/latest">
    <img src="https://img.shields.io/github/v/release/666OS/ClashMac?style=flat-square&logo=github&color=green" alt="Latest Release">
  </a>
  <a href="https://github.com/666OS/ClashMac/releases">
    <img src="https://img.shields.io/github/downloads/666OS/ClashMac/total?style=flat-square&logo=dropbox&logoColor=white&color=gold" alt="Downloads">
  </a>
  <a href="https://clashmac.app">
    <img src="https://img.shields.io/badge/Official-Website-orange?style=flat-square&logo=safari" alt="Official Website">
  </a>
  <a href="https://t.me/Pinched666">
    <img src="https://img.shields.io/badge/Telegram-Channel-blue?style=flat-square&logo=telegram">
  </a>
</p>

<p align="center">
  <a href="https://clashmac.app">
    <img src="assets/website.png" alt="ClashMac Website" width="800">
  </a>
</p>

## Preview
<table>
  <tr>
    <th>Dark</th>
    <th>Light</th>
  </tr>
  <tr>
    <td><img src="./assets/preview_dark.png" alt="Dark"></td>
    <td><img src="./assets/preview_light.png" alt="Light"></td>
  </tr>
  <tr>
    <td colspan="2" align="center"><img src="./assets/preview_dashboard.jpg" alt="Dashboard"></td>
  </tr>
</table>

## Features

- **Native Development**: Built with SwiftUI, deeply integrated with macOS
- **Dual Proxy Modes**: System Proxy + TUN Enhanced, complete traffic coverage
- **Standalone Dashboard**: Native Dashboard app with Proxies/Rules/Connections/Logs at a glance
- **Traffic Tracking**: 4-dimension statistics by Proxy/Process/Interface/Host, byte-level precision
- **Traffic Trends**: 7-day bar chart with daily average, usage patterns at a glance
- **Rule Statistics**: Visualize rule match counts, one-click reset
- **Privacy Mode**: One-click hide sensitive info like IP/nodes, share screenshots worry-free
- **One-Click Rules**: Add proxy rules for current webpage, supports major browsers
- **Zero Config**: Auto-complete DNS/TUN/GEO parameters, ready out of the box
- **Real-Time Stats**: Menu bar shows speed, connections, memory usage
- **Subscription Info**: Usage, expiry date, progress bar at a glance
- **Quick Switch**: Switch nodes directly from menu bar, one-click latency test
- **Subscription Management**: Remote config import, auto-update, smart naming
- **Drag & Drop**: Drop YAML config, auto-switch and apply
- **Config Pre-Check**: Auto-validate before import, pinpoint errors precisely
- **Video Boost**: Disable overseas QUIC, say goodbye to YouTube buffering
- **Parameter Override**: Unified config across subscriptions, no file modification
- **Crash Diagnosis**: Auto-identify issues, provide solutions
- **Shortcuts**: Rich keyboard shortcuts for efficient control
- **Lightweight**: Menu bar resident, minimal memory footprint
- **Customizable UI**: Show/hide menu items, create your own layout
- **Auto Update**: Detect new versions, one-click upgrade
- **Bilingual**: Auto-switch between English and Chinese
- **Password-Free**: Privileged helper handles auth, no password prompts

## System Requirements

| Feature | Minimum Version |
|---------|----------------|
| Basic Features | macOS 12.4+ |
| Dashboard/Traffic Stats/Privacy Mode | macOS 13.0+ |

## Download

Download the latest version from the [Releases page](https://github.com/666OS/ClashMac/releases/latest):

- **Apple Silicon (M1/M2/M3/M4)**: `ClashMac-v*-macos-arm64.zip`
- **Intel Mac**: `ClashMac-v*-macos-x86_64.zip`

**Compatible Configuration**: Please refer to [Test Configurations](https://github.com/666OS/YYDS/tree/main/mihomo/config)

**Installation Steps**:
1. Unzip the downloaded zip file
2. Drag `ClashMac.app` to the "Applications" folder
3. On first launch, right-click and select "Open" (to bypass security check)

**Tip**: Not sure which Mac you have? Click the  menu at the top left → About This Mac, and check the "Chip" information.

> **Note: Mac Gatekeeper may block unsigned applications**

### Solutions

#### Method 1: Allow in System Settings
1. Try to open ClashMac, click "Done" when the security warning appears
2. Open **System Settings** → **Privacy & Security**
3. Scroll down and find the message: "ClashMac was blocked from opening"
4. Click "Open Anyway" next to it
5. Click "Open Anyway" again in the popup dialog

#### Method 2: Remove Restrictions via Terminal
Enter in Terminal:

```bash
xattr -cr /Applications/ClashMac.app
```
Press Enter and reopen the application


#### Method 3: Remove Quarantine Attribute

Enter in Terminal:
```bash
xattr -d com.apple.quarantine /Applications/ClashMac.app
```
Press Enter and reopen the application

## Security Design

**Privileged Helper Security Hardening**: Fixed potential command injection vulnerabilities

- **Whitelist Path Validation**: Only allows kernel execution from `/Applications/ClashMac.app/`
- **Permission Tightening**: Restricted to admin user access only
- **POC Verified**: Attacks like `/bin/sh`, path traversal are all blocked

> *"Security is a process, not a product."* — Bruce Schneier

## Security & Privacy

This application runs entirely locally on macOS and does not collect or upload user data.  

Network access occurs only when explicitly configured by the user, or when the user manually checks for updates (downloads are served via GitHub).  

The application requests only the minimum system permissions required for its functionality.  

## License

ClashMac is a proprietary, closed-source application.  
Only binary releases are provided in this repository.

This project uses third-party open-source components.  
The full list of licenses is available at:

[THIRD_PARTY_LICENSES](https://github.com/666OS/ClashMac/blob/main/THIRD_PARTY_LICENSES.txt) 

## Acknowledgments

- [mihomo](https://github.com/MetaCubeX/mihomo)
- [Vernesong](https://github.com/vernesong/mihomo)
- [Zashboard](https://github.com/Zephyruso/zashboard)

## Star History
[![Star History Chart](https://api.star-history.com/svg?repos=666OS/ClashMac&type=Date)](https://star-history.com/#666OS/ClashMac&Date)

---

<p align="center">
  Made with ❤️ for macOS
</p>
