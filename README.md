# VoiceTel Phone

A modern, cross-platform SIP phone application available for Web, Desktop, and Mobile platforms. Built with WebRTC technology for crystal-clear voice communications.

## 🌟 Features

### Common across all platforms
- ✅ Secure SIP over TLS
- ✅ DTMF (RFC 2833 and SIP INFO)
- ✅ Caller ID, privacy toggle, and call history
- ✅ NAT-friendly ICE/STUN configuration
- ✅ Config persistence with local storage
- ✅ Troubleshooting log and diagnostics

### Platform-specific advantages

**Web Browser**
- 🌐 Instant launch links (tel: / custom scheme)
- 🚀 No installation required — perfect for kiosks & VDI
- 📱 Browser mic permissions guide

**Desktop (Windows, macOS, Linux)**
- 🖥️ System tray & global mute hotkey
- 🔄 Auto-start on login, auto-register
- 💪 Crash-resilient reconnect & logs

**Mobile (iOS, Android)**
- 🎧 Native audio routing & Bluetooth
- 📱 Background mode with quick actions

## 🚀 Quick Start

### Web Browser
Simply visit the [VoiceTel Phone Web App](https://phone.voicetel.com) and start calling immediately.

### Desktop Applications

#### Windows
1. Download the installer from [Windows Guide](https://phone.voicetel.com/windows.html)
2. Run the `.exe` or `.msi` installer
3. Launch from Start Menu

#### macOS
1. Download from [macOS Guide](https://phone.voicetel.com/macOS.html)
2. Open the `.dmg` and drag to Applications
3. Launch from Applications folder

#### Linux
1. Download from [Linux Guide](https://phone.voicetel.com/linux.html)
2. Choose your preferred package:
   - **AppImage**: Portable, works across most distros
   - **Debian/Ubuntu**: `.deb` package for APT integration
   - **Fedora/Red Hat**: `.rpm` package for DNF/yum integration

### Mobile Applications

#### iPhone
1. Follow the [iPhone Setup Guide](https://phone.voicetel.com/knowledge.html#iphone)
2. Enable Developer Mode in iOS Settings
3. Install via Xcode (Mac required)

#### Android
1. Follow the [Android Setup Guide](https://phone.voicetel.com/knowledge.html#android)
2. Enable Developer Options
3. Install via Android Studio

## 📋 Requirements

### Web Browser
- Modern browser with WebRTC support (Chrome, Firefox, Safari, Edge)
- Microphone permissions
- Stable internet connection

### Desktop
- **Windows**: Windows 10 or later
- **macOS**: macOS 10.15 or later
- **Linux**: Most modern distributions

### Mobile
- **iOS**: iOS 14 or later (Developer Mode required)
- **Android**: Android 8.0 or later (Developer Options required)

## 👤 User Accounts

### Getting Started
Before using VoiceTel Phone, you'll need to create an account:
- **Account Management**: [www.voicetel.com](http://www.voicetel.com)
- **Registration**: Sign up for a VoiceTel account
- **Account Setup**: Configure your SIP credentials and preferences

### SIP Credentials
You'll need the following information from your administrator:
- **Domain**: Your SIP domain (e.g., `tls.voicetel.com`)
- **Username**: Your 10-digit phone number
- **Password**: Your SIP password
- **Display Name**: Your preferred display name
- **Caller ID**: Optional 10-digit North American phone number

### Configuration Files

**Desktop Applications:**
- **Windows**: `%APPDATA%/VoiceTelPhone/voicetel.json`
- **macOS**: `~/Library/Application Support/VoiceTelPhone/voicetel.json`
- **Linux**: `~/.config/VoiceTelPhone/voicetel.json`

**System-wide (Desktop):**
- **macOS**: `/Library/Application Support/VoiceTelPhone/voicetel.json`
- **Linux**: `/etc/VoiceTelPhone/voicetel.json`

## 🛠️ Development

### Project Structure
```
phone/
├── index.html          # Landing page
├── phone.html          # Web application
├── knowledge.html      # Installation guides
├── windows.html        # Windows-specific guide
├── macOS.html          # macOS-specific guide
├── linux.html          # Linux-specific guide
└── README.md           # This file
```

### Building from Source

#### Web Application
The web application is a single HTML file with embedded CSS and JavaScript. No build process required.

#### Desktop Applications
Desktop applications are built using platform-specific tools:
- **Repository**: [voicetel/voicetel-phone-desktop](https://github.com/voicetel/voicetel-phone-desktop)
- **Windows**: Visual Studio / MSBuild
- **macOS**: Xcode
- **Linux**: CMake / Make

#### Mobile Applications
Mobile applications require platform-specific development environments:
- **Repository**: [voicetel/voicetel-phone-mobile](https://github.com/voicetel/voicetel-phone-mobile)
- **iOS**: Xcode (macOS required)
- **Android**: Android Studio

## 📚 Documentation

- [Installation Guides](https://phone.voicetel.com/knowledge.html)
- [Windows Setup](https://phone.voicetel.com/windows.html)
- [macOS Setup](https://phone.voicetel.com/macOS.html)
- [Linux Setup](https://phone.voicetel.com/linux.html)

## 🐛 Troubleshooting

### Common Issues

**Audio not working:**
- Check microphone permissions in system settings
- Verify correct input/output device selection
- Ensure audio drivers are up to date

**Registration failed:**
- Verify SIP credentials are correct
- Check network connectivity
- Ensure firewall allows SIP traffic (port 5060/5061)

**Call quality issues:**
- Check internet connection stability
- Verify NAT configuration
- Try disabling VPN if active

### Logs and Diagnostics

Desktop applications store logs in:
- **Windows**: `%APPDATA%/VoiceTelPhone/logs/`
- **macOS**: `~/Library/Logs/VoiceTelPhone/`
- **Linux**: `~/.local/share/VoiceTelPhone/logs/`

## 🤝 Support

- **Email**: support&#8203;@&#8203;voicetel&#8203;.&#8203;com
- **Issues**: Report bugs via GitHub Issues
  - [Web App Issues](https://github.com/voicetel/phone/issues)
  - [Desktop App Issues](https://github.com/voicetel/voicetel-phone-desktop/issues)
  - [Mobile App Issues](https://github.com/voicetel/voicetel-phone-mobile/issues)
- **Documentation**: [Knowledge Base](https://phone.voicetel.com/knowledge.html)

## 📄 License

Copyright © 2024 VoiceTel. All rights reserved.

## 🔗 Links

- **Website**: [www.voicetel.com](http://www.voicetel.com)
- **Web App**: [phone.voicetel.com](https://phone.voicetel.com)
- **Repositories**:
  - [Web App Source](https://github.com/voicetel/phone)
  - [Desktop App Source](https://github.com/voicetel/voicetel-phone-desktop)
  - [Mobile App Source](https://github.com/voicetel/voicetel-phone-mobile)
- **Status Page**: Available via the web application

---

**Version**: 3.5.5  
**Last Updated**: December 2024
