# FlowForge - TCP IP Spoofing & Network Tools
# FlowForge v1.0 - Release Notes

## 🎉 First Official Release

Welcome to the first stable release of FlowForge! FlowForge is a professional network tool that provides advanced TCP proxy and network utilities.

## 📋 Overview

**FlowForge** - TCP Proxy & Network Tool is a comprehensive network proxy tool developed for redirecting, manipulating network traffic, and creating mock servers. It can run in both GUI and CLI modes and is designed especially for test environments, development processes, and network analysis.

## ✨ Features

### 🔄 TCP Proxy Management
- **Forward Mode**: Redirect incoming TCP connections to another target
- **Fake Mode**: Send predefined hex data to incoming connections
- **Sequential Fake Mode**: Send hex data from a file sequentially
- Network adapter IP selection (dropdown + manual entry)
- Multiple proxy rule support
- Real-time connection monitoring

### 🌐 HTTP Mock Server
- Dynamic HTTP mock server creation
- Path matching (prefix and regex support)
- HTTP method filtering (GET, POST, PUT, DELETE, PATCH)
- Header and body content filtering
- Custom HTTP header addition
- Response delay configuration
- Text and file-based response support
- Multiple mock server management

### 🔒 HTTPS Proxy
- Integration with external HTTPS proxy tools (mitmproxy, etc.)
- Proxy profile management
- Windows WinHTTP proxy automatic configuration
- Live stdout/stderr log viewing
- Profile-based command management

### 🛡️ Windivert Integration
- Network traffic capture and redirection with Windows Windivert
- Multiple windivert rule management
- Automatic startup support
- Rule-based traffic redirection

### 🎯 DNS Spoofing
- Manipulate DNS requests
- Create custom DNS responses
- Domain-based redirection

### 🔍 Network Scanner
- Network scanning tools
- HTTP content analysis
- Packet capture and analysis
- Payload generation

### ⚔️ Offensive Security Tools
- **AISA**: Advanced network analysis
- **Behavior**: Behavior analysis
- **IDS Sim**: IDS simulation
- **Lateral Movement**: Lateral movement simulation
- **Stealth**: Stealth operation modes

### 📊 Data Packet Monitor (DPM)
- Real-time packet monitoring
- Network traffic analysis
- Packet-based filtering

### 🎨 Modern User Interface
- Professional dark theme
- Modern and intuitive GUI (Fyne v2)
- Colored log panel (level-based coloring)
- Real-time log viewing
- Log level selection (DEBUG, INFO, WARN, ERROR)
- New logs automatically added to the top
- Responsive and user-friendly design

### 💾 Data Management
- JSON format import/export
- Persistent settings storage
- Proxy profile management
- Windivert rule management
- Mock server rule management

### 🖥️ Platform Support
- **Windows** (primary platform)

### 🔧 CLI Mode
- Command-line interface
- Script support
- Suitable for automation

## 🚀 Installation

### Requirements
- Go 1.21 or higher
- Windows: GCC for CGO (MinGW or TDM-GCC) - Optional (for OpenGL)
- Can be compiled without CGO using software renderer mode

### Building

#### Software Renderer (Recommended - No CGO required)
```bash
build.bat software
```

#### OpenGL Renderer (Requires GCC)
```bash
build.bat
```

### Running

#### GUI Mode
```bash
FlowForge.exe
```

#### CLI Mode
```bash
FlowForge.exe --map "listen=0.0.0.0:27001,mode=forward,target=1.2.3.4:80" --log info
```

## 📝 License

This software is subject to the "End User Software License Agreement" displayed on first run. By using the software, you agree to this agreement.

## 👨‍💻 Developer

**Developer**: Ö.Ş  
**GitHub**: [https://github.com/02gur](https://github.com/02gur)  
**Programming Language**: Go (Golang)

## 🐛 Known Issues

- Linux and macOS support is experimental
- Some features only work on Windows (Windivert, WinHTTP proxy)

## 🔮 Future Releases

- Advanced log filtering
- More offensive security tools
- Plugin system
- Web-based interface option
- More protocol support

## 📞 Support

You can use GitHub Issues for questions and feedback.

## 🙏 Thanks

Thank you for using FlowForge!

---

**Note**: This software should only be used for legal and ethical purposes. Unauthorized network manipulation is prohibited.


