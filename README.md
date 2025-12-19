# TurboText - Text Shortcut Automation Tool


TurboText is a upgraded version of Key Hooker which is a lightweight Windows system tray application that automatically replaces text shortcuts with longer phrases as you type. Increase your productivity by creating custom text expansions for frequently used phrases, email addresses, phone numbers, and more.

## ✨ Features

- 🚀 **Instant text expansion** - Type shortcuts like `//name` to automatically expand to full text
- ⚙️ **Fully customizable** - Easily configure your own shortcuts in a simple text file
- 🎯 **System-wide functionality** - Works in any Windows application
- 🔄 **Hot reload** - Update shortcuts without restarting the application
- 📂 **Simple configuration** - Plain text file format for easy editing
- 🔒 **Privacy focused** - Runs locally, no data sent to servers
- 🖥️ **System tray integration** - Minimal UI, runs quietly in background

## 📦 Requirements

1. Windows 7 or later
2. Must have *.Net 10.0* Desktop Runtime installed

## 📦 Installation

1. Download the latest release from the [Releases page](https://github.com/tlstanjim/TurboText)
2. Extract the ZIP file to your preferred location
3. Run `TurboText.exe`
4. The application will create a default `shortcuts.txt` file on first run

## 🛠️ Configuration

Edit the `shortcuts.txt` file in the same directory as the executable:

```plaintext
//name=Your Full Name
//email=your.email@example.com
//phone=1 (555) 123-4567
//addr=123 Main Street, City, Country
//sig=Best regards,\nYour Name
```

### Format Rules:
- One shortcut per line in `shortcut=replacement` format
- Lines starting with `#` are treated as comments
- Empty lines are ignored
- Use `\n` for line breaks in replacement text
- Do not use symbols or anything without text or numbers

## 🎮 Usage

1. Launch TurboText (it will appear in your system tray)
2. Type any configured shortcut in any application
3. Watch as it automatically expands to your predefined text

**Example:** Typing `//email` becomes `your.email@example.com`

## ⌨️ Default Shortcuts

The application comes with these default shortcuts:

## 🔧 Managing the Application

- **Right-click the system tray icon** to access the menu
- Select **"Edit"** to Open `shortcuts.txt`
- Select **"Reload"** to apply changes to shortcuts.txt
- Select **"Exit"** to close the application

## 🐛 Troubleshooting

1. **Shortcuts not expanding?**
   - Ensure the application is running (check system tray)
   - Verify your shortcuts.txt format is correct
   - Use the "Reload Shortcuts" option from the tray menu

2. **Application won't start?**
   - Ensure you have *.NET 10.0* Desktop Runtime installed
   - Check if another instance is already running

3. **Performance issues?**
   - Limit your shortcuts to a reasonable number (under 100) cause it can feel buggy
   - Avoid using expanded name of same shortcuts like `//abc`*main* and `//abcd`*expanded* as it can override shortcuts
   - Give each shortcut and unique name
   - Avoid extremely long replacement texts

## 📝 License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.

## 🤝 Contributing

Contributions, issues, and feature requests are welcome! Feel free to [contact me](tls.tanjim@gmail.com)


---

**Note:** TurboText uses low-level keyboard hooks which may be detected by some security software as a keylogger. This is a false positive - the application only monitors for specific shortcut patterns and does not record or transmit your keystrokes.

---

<div align="center">
  
If you find this tool useful, please consider giving it a ⭐ on GitHub!

</div>
