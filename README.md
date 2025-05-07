# 🚀 Python to EXE Converter - Enhanced

A powerful GUI application that simplifies converting Python scripts to standalone executables using PyInstaller, with automatic error detection and resolution.

![Python to EXE Converter](https://img.shields.io/badge/Python-to_EXE-blue)
![PyInstaller](https://img.shields.io/badge/PyInstaller-Enhanced-green)
![Platform](https://img.shields.io/badge/Platform-Windows-lightgrey)

## ✨ Features

### 🔄 Automatic Dependency Analysis
- 🔍 Automatically scans Python files for imports
- 📊 Pre-emptively identifies problematic packages
- 🧩 Suggests hidden imports based on detected dependencies

### 🛠️ Enhanced Error Detection and Resolution
- 🔧 Automatically detects and fixes common PyInstaller errors
- 🔄 Multiple retry strategies for different types of errors
- 🧪 Improved pattern matching for detecting missing modules
- 🔌 Detection and handling for DLL errors

### 📊 Progress Tracking
- 📈 Real-time progress updates with percentage completion
- 🔔 Notifications when conversion is complete
- 📝 Detailed logs of the conversion process

### ⚙️ Performance Optimization
- ⚡ Fast Mode for skipping non-essential analysis steps
- 🔄 Selective module exclusion based on actual imports
- ⏱️ Timeout detection for hanging processes

### 🔔 Notification System
- 🔊 Sound alerts when conversion completes or fails
- 💬 System tray notifications
- ⏰ Timestamps for all events

### 🔄 PyInstaller Version Management
- 🔍 Detects outdated PyInstaller versions
- 📝 Shows update instructions in the GUI
- 📋 One-click copy of update commands

### 🎨 User-Friendly Interface
- 📑 Tabbed interface for basic and advanced options
- 🔧 Troubleshooting guide with common problems and solutions
- 📋 Log viewer with save and clear options

## 📋 Requirements

- Python 3.6 or higher
- PyInstaller 5.6.2 or higher (recommended)
- PyQt6
- Other dependencies listed in `requirements.txt`

## 🚀 Installation

1. Clone this repository or download the source code:
```bash
git clone https://github.com/zinzied/python-to-exe-enhanced.git
cd python-to-exe-enhanced
```

2. Install the required dependencies:
```bash
pip install -r requirements.txt
```

3. Run the application:
```bash
python py2exe.py
```

## 📖 Usage

### Basic Usage

1. 📂 Select a Python file to convert
2. 📁 Choose an output directory
3. ⚙️ Configure basic options:
   - Output type (single executable or folder)
   - Window mode (console or windowed)
4. ✅ Enable auto-detect dependencies and auto-fix errors (recommended)
5. 🚀 Click "Convert to EXE"

### Advanced Options

- 🧩 Add hidden imports manually or let the app detect them
- 📁 Add additional files and directories to include in the executable
- 🖼️ Specify an icon for the executable
- ⚙️ Configure additional PyInstaller options
- 📝 Generate and edit a .spec file for more control

### Performance Options

- ⚡ **Fast Mode**: Speeds up conversion by skipping non-essential analysis steps
- 🔄 **Skip Validation**: Further speeds up conversion but may be less reliable
- 📊 **Verbose Output**: Shows detailed output from PyInstaller for debugging

### Notification Options

- 🔊 Enable/disable sound notifications
- 💬 System tray notifications when conversion completes

## 🔧 Troubleshooting

The application includes a dedicated troubleshooting tab with solutions to common problems:

- 📦 Missing modules
- 🔌 DLL load failures
- 🚫 Failed execution
- 🔄 Recursion errors
- 🖼️ Qt library issues
- 🧩 Tkinter issues
- 📁 File not found errors
- 🔒 Permission issues

## 📋 Logs

- 📊 View real-time logs during conversion
- 💾 Save logs for further analysis
- 🧹 Clear logs when needed

## 🔄 Version Checking

The application automatically checks if your PyInstaller version is up to date:

- 🔍 Detects the installed version of PyInstaller
- ⚠️ Shows a warning if the version is outdated
- 📝 Provides the exact command to update PyInstaller
- 📋 Allows copying the update command with one click

## 📝 License

This project is licensed under the MIT License - see the LICENSE file for details.

## 🙏 Acknowledgements

- [PyInstaller](https://www.pyinstaller.org/) for the amazing tool that makes Python to EXE conversion possible
- [PyQt6](https://www.riverbankcomputing.com/software/pyqt/) for the GUI framework
- All contributors and users who have provided feedback and suggestions

## 🤝 Contributing

Contributions are welcome! Please feel free to submit a Pull Request.

1. Fork the repository
2. Create your feature branch (`git checkout -b feature/amazing-feature`)
3. Commit your changes (`git commit -m 'Add some amazing feature'`)
4. Push to the branch (`git push origin feature/amazing-feature`)
5. Open a Pull Request
