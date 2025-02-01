# Kismet Core Installer

This repository contains installers for the Kismet Core application across multiple platforms (macOS, Windows, and Linux).

## Platform-Specific Installation Instructions

### macOS Installation

1. Navigate to the `x86_64-apple-darwin/release` directory
2. Locate the `kismet-installer.dmg` file
3. Double-click the DMG file to mount it
4. Drag the Kismet Core application to your Applications folder
5. First time running: Right-click the application and select "Open" to bypass macOS security

### Windows Installation

1. Navigate to the `x86_64-pc-windows-gnu/release` directory
2. Download the installer executable
3. Run the installer with administrator privileges
4. Follow the installation wizard prompts
5. After installation, you can launch Kismet Core from the Start Menu

### Linux Installation

1. Navigate to the `x86_64-unknown-linux-gnu/release` directory
2. Make the installer executable:
   ```bash
   chmod +x kismet-core-installer
   ```
3. Run the installer:
   ```bash
   ./kismet-core-installer
   ```
4. Follow the terminal prompts to complete installation

## System Requirements

### macOS

- macOS 10.15 (Catalina) or later
- x86_64 processor
- 4GB RAM minimum
- 500MB free disk space

### Windows

- Windows 10 or later
- x86_64 processor
- 4GB RAM minimum
- 500MB free disk space

### Linux

- Modern Linux distribution (Ubuntu 20.04+, Fedora 34+, etc.)
- x86_64 processor
- 4GB RAM minimum
- 500MB free disk space

## Troubleshooting

### macOS

- If you see "app is damaged" message, go to System Preferences > Security & Privacy and allow the application
- If installation fails, ensure you have adequate disk space and appropriate permissions

### Windows

- Run the installer as administrator if you encounter permission issues
- If Windows SmartScreen blocks the installer, click "More info" and "Run anyway"

### Linux

- Ensure you have necessary dependencies installed:
  ```bash
  # Ubuntu/Debian
  sudo apt-get update
  sudo apt-get install libssl-dev

  # Fedora
  sudo dnf install openssl-devel
  ```

## Support

If you encounter any issues during installation:

1. Check our [GitHub Issues](https://github.com/kismet-dao/installer/issues) for known problems
2. Create a new issue with details about your system and the error message
3. For urgent assistance, contact our support team

## Building from Source

For instructions on building the installers from source, please see our [Build Documentation](BUILD.md).