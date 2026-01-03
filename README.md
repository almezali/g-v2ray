# G-v2ray Professional Edition

<p align="center">
  <strong>🚀 Advanced V2Ray/Xray GUI Client for Linux</strong>
</p>

<p align="center">
  <a href="#features">Features</a> •
  <a href="#installation">Installation</a> •
  <a href="#requirements">Requirements</a> •
  <a href="#usage">Usage</a> •
  <a href="#build">Build</a> •
  <a href="#license">License</a>
</p>

---

## 📖 Overview

**G-v2ray Professional Edition** is a feature-rich, user-friendly GUI application for managing V2Ray and Xray connections on Linux. Built with GTK3 and Python, it provides an intuitive interface for configuring, connecting, and monitoring V2Ray/Xray proxies with advanced features like automatic server fetching, latency testing, system proxy integration, and comprehensive connection statistics.

### ✨ Key Highlights

- 🎯 **Universal Compatibility**: Works with both V2Ray and Xray cores
- 🌍 **Free Server Discovery**: Automatically fetch and test free V2Ray servers
- ⚡ **Smart Auto-Reconnect**: Keeps you connected with intelligent reconnection
- 📊 **Real-time Statistics**: Monitor connection speed, latency, and data usage
- 🔧 **Auto-Dependency Management**: Automatically detects and installs required packages
- 🎨 **Modern UI**: Clean, professional interface with dark/light theme support
- 🔐 **System Integration**: Automatic system proxy configuration

---

## 🎯 Features

### Core Features

#### 🔌 Connection Management
- ✅ VMess protocol support with full configuration options
- ✅ Multiple profile management with search and filtering
- ✅ Quick connect/disconnect with status indicators
- ✅ Automatic reconnection on connection drops
- ✅ Connection uptime tracking and monitoring
- ✅ Real-time connection status updates

#### 🌐 Free Server Integration
- ✅ Fetch free V2Ray servers from multiple public sources
- ✅ Automatic server validation and testing
- ✅ Bulk latency testing for all servers
- ✅ Server filtering and search capabilities
- ✅ Quality indicators (Excellent/Good/Fair/Poor)
- ✅ One-click server import to profiles

#### 📊 Advanced Statistics
- ✅ Real-time data usage tracking (upload/download)
- ✅ Connection latency monitoring (avg/min/max)
- ✅ Public IP detection and change notification
- ✅ Session uptime display
- ✅ Network speed indicators
- ✅ Comprehensive logging system

#### ⚙️ System Integration
- ✅ Automatic system proxy configuration (GNOME)
- ✅ System tray integration with AppIndicator
- ✅ Minimize to tray functionality
- ✅ Desktop notifications for connection events
- ✅ Auto-start on system boot (optional)
- ✅ Configurable SOCKS5 and HTTP proxy ports

#### 🛠️ Configuration & Profiles
- ✅ VMess link import (vmess://)
- ✅ Manual profile configuration
- ✅ Profile import/export (JSON)
- ✅ Profile editing and management
- ✅ Connection profile validation
- ✅ Custom DNS server configuration

#### 🎨 User Interface
- ✅ Clean, modern GTK3 interface
- ✅ Dark/Light theme support
- ✅ Searchable profile list
- ✅ Real-time log viewer
- ✅ Intuitive connection controls
- ✅ Responsive design with proper scaling

#### 🔧 Advanced Options
- ✅ Configurable reconnection delay
- ✅ Custom proxy port configuration
- ✅ Log level adjustment
- ✅ DNS server customization
- ✅ Network type support (TCP/WS/H2/gRPC)
- ✅ TLS/Security configuration

#### 📦 Package Management
- ✅ Automatic dependency detection
- ✅ Cross-distribution package installation
- ✅ Smart core executable detection (V2Ray/Xray)
- ✅ User-friendly installation prompts
- ✅ Support for major Linux distributions

---

## 💻 System Requirements

### Minimum Requirements

#### Hardware
- **CPU**: 1 GHz dual-core processor or better
- **RAM**: 512 MB minimum (1 GB recommended)
- **Disk Space**: 100 MB for application + 50 MB for dependencies
- **Display**: 1024x768 resolution minimum

#### Software
- **Linux Kernel**: 3.10 or higher
- **Python**: 3.7 or higher
- **GTK**: 3.20 or higher
- **V2Ray/Xray Core**: Any recent version

### Supported Linux Distributions

#### 🐧 Arch Linux & Derivatives
- ✅ Arch Linux
- ✅ Manjaro
- ✅ EndeavourOS
- ✅ ArcoLinux
- ✅ Garuda Linux

**Package Manager**: `pacman`

#### 🎩 Red Hat & Derivatives
- ✅ Fedora (35+)
- ✅ RHEL (8+)
- ✅ CentOS (8+)
- ✅ Rocky Linux
- ✅ AlmaLinux

**Package Managers**: `dnf`, `yum`

#### 🌊 Debian & Derivatives
- ✅ Debian (10+)
- ✅ Ubuntu (20.04+)
- ✅ Linux Mint (20+)
- ✅ Pop!_OS
- ✅ Elementary OS
- ✅ Zorin OS
- ✅ MX Linux

**Package Manager**: `apt`

#### 🦎 openSUSE
- ✅ openSUSE Leap
- ✅ openSUSE Tumbleweed

**Package Manager**: `zypper`

#### 🎭 Other Distributions
- ✅ Gentoo
- ✅ Void Linux
- ✅ Solus
- ✅ Any distribution with GTK3 support

---

## 📥 Installation

### Method 1: AppImage (Recommended)

The AppImage version includes all dependencies and works on all major Linux distributions.

```bash
# Download the latest AppImage
wget https://github.com/almezali/g-v2ray/G-V2Ray-2.1-x86_64.AppImage

# Make it executable
chmod +x G-V2Ray-2.1-x86_64.AppImage

# Run the application
./G-V2Ray-2.1-x86_64.AppImage
```

### Method 2: Arch User Repository (AUR)

For Arch Linux users, G-v2ray is available in the AUR:

```bash
# Using yay
yay -S g-v2ray-appimage

# Using paru
paru -S g-v2ray-appimage

# Using pamac
pamac install g-v2ray-appimage
```


## 🔧 Dependencies

### Automatic Installation

G-v2ray **automatically detects and offers to install** missing dependencies on first run. The installation wizard supports:

- 🔹 Arch Linux: `pacman`
- 🔹 Debian/Ubuntu: `apt`
- 🔹 Fedora: `dnf`
- 🔹 RHEL/CentOS: `yum`
- 🔹 openSUSE: `zypper`

### Core Dependencies

#### Required
- **Python 3** (`python3`)
- **GTK 3** (`gtk3`, `python3-gi`)
- **GObject Introspection** (`python3-gi-cairo`, `gir1.2-gtk-3.0`)
- **V2Ray or Xray** (`v2ray` or `xray`)

#### Optional (but recommended)
- **AppIndicator3** (`gir1.2-appindicator3-0.1`) - For system tray
- **QRCode** (`python-qrcode`) - For QR code generation
- **Pillow** (`python-pillow`) - For image processing

### Manual Installation Examples

#### Arch Linux
```bash
sudo pacman -S python python-gobject gtk3 v2ray
# Optional
sudo pacman -S libappindicator-gtk3 python-qrcode python-pillow
```

#### Ubuntu/Debian
```bash
sudo apt update
sudo apt install python3 python3-gi python3-gi-cairo gir1.2-gtk-3.0 v2ray
# Optional
sudo apt install gir1.2-appindicator3-0.1 python3-qrcode python3-pil
```

#### Fedora
```bash
sudo dnf install python3 python3-gobject gtk3 v2ray
# Optional
sudo dnf install libappindicator-gtk3 python3-qrcode python3-pillow
```

---

## 🚀 Usage

### First Launch

1. **Start the application**
   ```bash
   ./G-V2Ray-2.1-x86_64.AppImage
   ```

2. **Dependency Check**
   - G-v2ray will automatically check for required dependencies
   - If V2Ray/Xray is missing, it will offer to install it
   - Click "Yes" to allow automatic installation (requires sudo)

3. **Add a Profile**
   - Click "➕ Add Profile" in the sidebar
   - Paste a VMess link (vmess://...)
   - Or enter server details manually
   - Click "Add" to save

### Connecting to a Server

1. **Select a Profile**
   - Click on any profile in the sidebar
   - Profile details will be displayed

2. **Test Connection (Optional)**
   - Click "🔍 Test Latency" to check server response
   - View latency results before connecting

3. **Connect**
   - Click "▶ Connect" button
   - Wait for connection to establish
   - Status indicator will turn green

4. **Monitor Connection**
   - View real-time IP address
   - Check connection uptime
   - Monitor data usage and latency
   - Review logs for detailed information

### Using Free Servers

1. **Fetch Free Servers**
   - Click "🌍 Get Free Servers" button
   - Wait while servers are fetched from multiple sources
   - Servers will be displayed with details

2. **Test Servers**
   - Click "⚡ Test All Latency" to test all servers
   - Or click individual "Test" buttons
   - Servers are color-coded by quality:
     - 🟢 Green: Excellent (<200ms)
     - 🟠 Orange: Good (200-500ms)
     - 🔴 Red: Fair/Poor (>500ms)

3. **Filter and Select**
   - Use search box to filter servers
   - Select/deselect servers with checkboxes
   - Click "Add Selected" to import to profiles

### System Proxy Configuration

G-v2ray automatically configures system proxy on connection (GNOME/Ubuntu):

- **HTTP Proxy**: `127.0.0.1:8080`
- **SOCKS5 Proxy**: `127.0.0.1:1080`

For manual configuration or other desktop environments:

1. Go to System Settings → Network → Proxy
2. Set Manual proxy:
   - HTTP Proxy: `127.0.0.1:8080`
   - SOCKS Host: `127.0.0.1:1080`

### Settings Configuration

Click menu (⋮) → Settings to configure:

- ⚙️ **Auto-reconnect**: Enable automatic reconnection
- ⏱️ **Reconnect delay**: Set delay between reconnection attempts
- 🔔 **Notifications**: Enable/disable system notifications
- 🖥️ **System proxy**: Auto-configure system proxy on connect
- 🎨 **Theme**: Choose Auto/Light/Dark theme
- 🔌 **Proxy ports**: Customize SOCKS and HTTP ports

### Profile Management

#### Import/Export
- **Export**: Click "📤 Export" to save profiles as JSON
- **Import**: Click "📥 Import" to load profiles from JSON file

#### Edit Profile
- Select a profile
- Click "✏️ Edit" to modify settings
- Update server address, port, or other details
- Click "Save" to apply changes

#### Delete Profile
- Select a profile
- Click "🗑️ Delete" to remove
- Confirm deletion

### System Tray

When minimized, G-v2ray stays in system tray:

- **Show Window**: Click to restore window
- **Connect**: Quick connect to selected profile
- **Disconnect**: Terminate connection
- **Quit**: Exit application

---

## 📸 Screenshots

### Main Interface
The main interface provides a clean and intuitive layout with profile management on the left and connection details on the right.


  ![Main Interface](https://github.com/almezali/g-v2ray/blob/main/Screenshot-n1.png)


**Features shown:**
- Profile list with search functionality
- Connection status with real-time IP display
- Statistics showing uptime, data usage, and latency
- Integrated log viewer
- Quick action buttons

### Free Servers Discovery
Automatically fetch and test free V2Ray servers from multiple sources with one click.


  ![Free Servers](https://github.com/almezali/g-v2ray/blob/main/Screenshot-n2.png)


**Features shown:**
- Multiple server sources
- Real-time latency testing
- Quality indicators (color-coded)
- Server filtering and search
- Bulk selection and import

---

## 📝 Configuration Files

G-v2ray stores configuration in `~/.config/g-v2ray/`:

- **profiles.json**: Saved connection profiles
- **settings.json**: Application settings
- **v2ray.log**: Connection and application logs
- **active.json**: Current active V2Ray configuration

### Backup Your Data

```bash
# Backup profiles and settings
cp -r ~/.config/g-v2ray ~/g-v2ray-backup

# Restore from backup
cp -r ~/g-v2ray-backup ~/.config/g-v2ray
```

---

## 🔍 Troubleshooting

### Connection Issues

**Problem**: Cannot connect to server
- ✅ Verify server details are correct
- ✅ Test server latency before connecting
- ✅ Check V2Ray/Xray logs for errors
- ✅ Ensure firewall allows outbound connections

**Problem**: V2Ray/Xray not found
- ✅ Install V2Ray or Xray: `sudo pacman -S v2ray` or `sudo pacman -S xray`
- ✅ Restart application after installation
- ✅ Check PATH includes core executable

### System Proxy Issues

**Problem**: System proxy not set automatically
- ✅ Enable "Auto set system proxy" in Settings
- ✅ Manually configure proxy in system settings
- ✅ Use proxy configuration: HTTP `127.0.0.1:8080`, SOCKS `127.0.0.1:1080`

### UI/Display Issues

**Problem**: Interface not displaying correctly
- ✅ Update GTK3: `sudo pacman -S gtk3`
- ✅ Try different theme in Settings
- ✅ Check display scaling settings

**Problem**: Tray icon not showing
- ✅ Install AppIndicator: `sudo pacman -S libappindicator-gtk3`
- ✅ Enable system tray in desktop environment
- ✅ Restart application

### Log Files

Check logs for detailed error information:

```bash
# View application logs
cat ~/.config/g-v2ray/v2ray.log

# Monitor logs in real-time
tail -f ~/.config/g-v2ray/v2ray.log
```

---

## 🤝 Contributing

Contributions are welcome! Here's how you can help:

1. 🍴 Fork the repository
2. 🔨 Create a feature branch: `git checkout -b feature/AmazingFeature`
3. 💾 Commit changes: `git commit -m 'Add AmazingFeature'`
4. 📤 Push to branch: `git push origin feature/AmazingFeature`
5. 🎉 Open a Pull Request


---

## 📄 License

This project is licensed under the **MIT License** - see the [LICENSE](LICENSE) file for details.

```
MIT License

Copyright (c) 2026 Mahmoud Almezali

Permission is hereby granted, free of charge, to any person obtaining a copy
of this software and associated documentation files (the "Software"), to deal
in the Software without restriction, including without limitation the rights
to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
copies of the Software, and to permit persons to whom the Software is
furnished to do so, subject to the following conditions:

The above copyright notice and this permission notice shall be included in all
copies or substantial portions of the Software.

THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
SOFTWARE.
```

---

## 🌟 Acknowledgments

- **V2Ray Project** - Core proxy technology
- **Xray Project** - Enhanced V2Ray fork
- **GTK Project** - UI framework
- **Free V2Ray Providers** - Community-maintained server lists
- **Linux Community** - Testing and feedback

---

## 📞 Support

- 🐛 **Bug Reports**: [GitHub Issues](https://github.com/almezali/g-v2ray/issues)
- 💬 **Discussions**: [GitHub Discussions](https://github.com/almezali/g-v2ray/discussions)


---

## 🗺️ Roadmap

### Planned Features

- [ ] Shadowsocks protocol support
- [ ] Trojan protocol support
- [ ] Traffic routing rules editor
- [ ] Subscription URL support
- [ ] Connection speed graphs
- [ ] Multiple language support
- [ ] QR code import/export
- [ ] Backup/restore functionality
- [ ] Profile groups/folders
- [ ] Advanced DNS configuration
- [ ] Split tunneling support
- [ ] Custom routing rules

---

## 📊 Version History

### Version 2.1 (Current)
- ✨ Added free server discovery feature
- ✨ Implemented bulk latency testing
- ✨ Added automatic dependency installation
- ✨ Improved system proxy integration
- ✨ Enhanced connection statistics
- 🐛 Fixed reconnection issues
- 🐛 Improved error handling

### Version 2.0
- 🎉 Complete UI redesign
- ✨ Added profile management
- ✨ Implemented system tray
- ✨ Added auto-reconnect
- ✨ Real-time statistics

### Version 1.0
- 🎉 Initial release
- ✅ Basic V2Ray connection
- ✅ Simple profile management

---

<p align="center">
  <strong>⭐ Star this project if you find it useful! ⭐</strong>
</p>

<p align="center">
  Made with ❤️ by <a href="https://github.com/almezali">Mahmoud Almezali</a>
</p>
