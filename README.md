# 🚀 Python to EXE Converter - Enhanced

A powerful GUI application that simplifies converting Python scripts to standalone executables using PyInstaller, featuring intelligent error detection and auto-fixing, automatic hidden import resolution, comprehensive notifications, and PyInstaller version management. The converter automatically solves common PyInstaller errors without requiring manual intervention.

![Python to EXE Converter](https://img.shields.io/badge/Python-to_EXE-blue)
![PyInstaller](https://img.shields.io/badge/PyInstaller-Enhanced-green)
![Platform](https://img.shields.io/badge/Platform-Windows-lightgrey)

## ✨ Features

### 🔄 Intelligent Dependency Analysis and Hidden Imports
- 🔍 **Smart Import Detection**: Automatically scans Python files to identify all imports and dependencies
- 📊 **Problematic Package Database**: Contains a comprehensive database of packages known to cause PyInstaller issues
- 🧩 **Automatic Hidden Import Resolution**: Identifies and adds necessary hidden imports without manual intervention
- 🔗 **Submodule Detection**: Recognizes when specific submodules need to be included as hidden imports
- 📦 **Package Relationship Analysis**: Understands dependencies between packages to ensure complete inclusion
- 🧠 **Learning from Errors**: Adds missing imports discovered during failed conversion attempts

### 🛠️ Advanced Error Detection and Auto-Fixing
- 🔧 **Intelligent Error Analysis**: Automatically detects, diagnoses, and fixes common PyInstaller errors in real-time
- 🔄 **Multi-Attempt Conversion**: Makes up to 3 conversion attempts, applying incremental fixes between attempts
- 🧪 **Pattern Recognition**: Uses advanced regex patterns to identify specific error types in conversion output
- 🔌 **DLL Error Resolution**: Automatically detects missing DLLs and adds them from System32 when available
- 🔍 **Detailed Error Logging**: Provides clear explanations of errors and the fixes being applied
- 💡 **Solution Suggestions**: Offers specific solutions for errors that can't be automatically fixed

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
- 💬 System tray notifications with completion status
- ⏰ Timestamps for all conversion events
- 🖥️ Desktop notifications when process finishes

### 🔄 PyInstaller Version Management
- 🔍 Automatically detects PyInstaller installation status
- ⚠️ Warns about outdated or missing PyInstaller versions
- 📝 Shows detailed update instructions in the GUI
- 📋 One-click copy of update commands
- 🔄 "Check Again" button to verify installation after updating

### 🎨 User-Friendly Interface
- 📑 Tabbed interface for basic, advanced, logs, and troubleshooting
- 🔧 Comprehensive troubleshooting guide with common problems and solutions
- 📋 Log viewer with save and clear options
- 🔍 Detailed error analysis and suggestions

## 📋 Requirements

- Python 3.6 or higher
- PyInstaller 5.6.2 or higher (recommended)
- PyQt5 (version 5.15.0 or higher)
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

#### 🧩 Hidden Imports Management
- **Automatic Detection**: Let the app automatically detect and add required hidden imports
- **Manual Addition**: Add specific hidden imports that you know are needed
- **Import Database**: Benefit from the app's database of known problematic packages and their required imports
- **Dynamic Learning**: The app learns from conversion errors and adds missing imports automatically

#### 📁 Additional Files and Resources
- **Multiple File Selection**: Select multiple files at once to include in your executable
- **Directory Support**: Add entire directories with automatic destination path assignment
- **Destination Path Editing**: Double-click any item to edit its destination path
- **Batch Operations**: Select multiple items for removal or editing

#### ⚙️ Other Advanced Options
- 🖼️ Specify an icon for the executable
- 🧹 Clean build files before building (--clean)
- ✂️ Strip binaries to reduce size (--strip)
- 🔒 Request UAC elevation (--uac-admin)
- 📝 Generate and edit a .spec file for more control
- ⌨️ Add custom command-line options

### Performance Options

- ⚡ **Fast Mode**: Speeds up conversion by skipping non-essential analysis steps
- 🔄 **Skip Validation**: Further speeds up conversion but may be less reliable
- 📊 **Verbose Output**: Shows detailed output from PyInstaller for debugging

### Notification Options

- 🔊 Enable/disable sound notifications for completion and errors
- 💬 System tray notifications with status information
- ⏰ Timestamps for all conversion events
- 🔔 Visual alerts for important events

## 🔧 Automatic Error Detection and Resolution

The application includes powerful error detection and auto-fixing capabilities:

### 🔍 Automatically Detected Errors

The converter automatically detects and fixes these common errors:

- 📦 **Missing Module Errors**: Identifies and adds required hidden imports
- 🔌 **DLL Load Failures**: Detects missing DLLs and adds them from System32
- 🚫 **Failed Execution Errors**: Adds debug options to get more information
- 🔄 **Recursion Errors**: Excludes problematic modules causing circular imports
- 🖼️ **Qt Binding Conflicts**: Special handling for multiple Qt frameworks (PyQt5/PyQt6)
- 🧩 **Tkinter Issues**: Adds necessary tkinter submodules as hidden imports
- 📁 **File Not Found Errors**: Suggests adding missing files as data files
- 🔤 **Unicode/Encoding Errors**: Adds appropriate encoding options
- 💻 **Terminal Application Issues**: Detects terminal applications and warns if using windowed mode

### 💡 Error Resolution Process

1. **Error Detection**: Parses conversion output using regex patterns to identify specific errors
2. **Solution Application**: Automatically applies the appropriate fix based on error type
3. **Retry Mechanism**: Makes up to 3 conversion attempts, applying fixes between attempts
4. **Detailed Logging**: Provides clear explanations of errors and fixes in the logs

### 📋 Comprehensive Troubleshooting Tab

The dedicated troubleshooting tab provides detailed solutions for issues that may require manual intervention:

- 📚 **Common Problems Database**: Extensive collection of PyInstaller issues and solutions
- 🔍 **Error Lookup**: Find solutions for specific error messages
- 🖼️ **Special Qt Section**: Detailed guidance for handling Qt framework issues
- 🔧 **Step-by-Step Solutions**: Clear instructions for resolving complex problems

## 📋 Logs

- 📊 View real-time logs during conversion
- 💾 Save logs for further analysis
- 🧹 Clear logs when needed

## 🔄 Version Checking

The application automatically checks if your PyInstaller version is up to date:

- 🔍 Detects the installed version of PyInstaller (or if it's missing)
- ⚠️ Shows a warning if the version is outdated or not installed
- 📝 Provides the exact command to install or update PyInstaller
- 📋 Allows copying the update command with one click
- 🔄 "Check Again" button to verify installation after updating
- 🛡️ Prevents conversion attempts with incompatible PyInstaller versions

## 🔄 Recent Updates

### ✨ New Features

#### 🛠️ Enhanced Error Detection and Auto-Fixing
- **Intelligent Error Analysis**: The converter now automatically detects and fixes common PyInstaller errors
- **Multi-Attempt Conversion**: Makes up to 3 conversion attempts, applying incremental fixes between attempts
- **Detailed Error Logging**: Provides clear explanations of errors and the fixes being applied

#### 💻 Terminal Application Support
- **Automatic Detection**: Identifies terminal applications by analyzing code patterns
- **Smart Mode Selection**: Warns if a terminal application is being built with windowed mode
- **Comprehensive Guidance**: Detailed troubleshooting section for terminal application issues
- **Path Resolution Help**: Code templates for handling file paths correctly in packaged applications

#### 🧩 Improved Hidden Imports Management
- **Automatic Detection**: Significantly improved detection of required hidden imports
- **Expanded Database**: Added more known problematic packages and their required imports
- **Dynamic Learning**: The app now learns from conversion errors and adds missing imports automatically

#### 📁 Enhanced File Management
- **Multiple File Selection**: Now supports selecting multiple files at once
- **Improved Directory Handling**: Better support for adding directories with automatic destination paths
- **Destination Path Editing**: Double-click any item to edit its destination path

## 📝 License

This project is licensed under the MIT License - see the LICENSE file for details.

## 🙏 Acknowledgements

- [PyInstaller](https://www.pyinstaller.org/) for the amazing tool that makes Python to EXE conversion possible
- [PyQt5](https://www.riverbankcomputing.com/software/pyqt/) for the GUI framework
- All contributors and users who have provided feedback and suggestions

## 🤝 Contributing

Contributions are welcome! Please feel free to submit a Pull Request.

1. Fork the repository
2. Create your feature branch (`git checkout -b feature/amazing-feature`)
3. Commit your changes (`git commit -m 'Add some amazing feature'`)
4. Push to the branch (`git push origin feature/amazing-feature`)
5. Open a Pull Request
