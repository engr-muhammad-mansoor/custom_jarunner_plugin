# JARunner - VS Code Extension

A lightweight Visual Studio Code extension that allows you to quickly run JAR files directly from your workspace with a simple keyboard shortcut.

## 🚀 Features

- **Quick JAR Execution**: Run JAR files instantly with a keyboard shortcut (`Ctrl+Alt+J` / `Cmd+Alt+J`)
- **Integrated Terminal**: Automatically opens a dedicated terminal for JAR execution
- **Cross-Platform**: Works on Windows, macOS, and Linux
- **Simple & Lightweight**: Minimal setup required

## 📋 Requirements

- Visual Studio Code 1.85.0 or higher
- Java Runtime Environment (JRE) installed and accessible via command line

## 🔧 Installation

Clone the repository and install dependencies:

```bash
git clone https://github.com/engr-muhammad-mansoor/custom_jarunner_plugin.git
cd custom_jarunner_plugin
npm install
npm run compile
```

Press `F5` in VS Code to launch the Extension Development Host and test the extension.

## 📖 Usage

Press `Ctrl+Alt+J` (Windows/Linux) or `Cmd+Alt+J` (macOS), or use the Command Palette to run "JarFileRun" command. The extension will execute the configured JAR file in a dedicated terminal.

**Note**: Update the JAR file path in `src/extension.ts` before use. Future versions will include a file picker for dynamic JAR file selection.

## 🛠️ Development

### Build Commands

- `npm run compile` - Compile TypeScript to JavaScript
- `npm run watch` - Watch for changes and recompile
- `npm run lint` - Run ESLint
- `npm test` - Run tests

### Project Structure

```
custom_jarunner_plugin/
├── src/
│   ├── extension.ts      # Main extension code
│   └── test/
│       └── extension.test.ts
├── package.json          # Extension manifest
├── tsconfig.json         # TypeScript configuration
└── README.md
```

## 🤝 Contributing

Contributions are welcome! Please feel free to submit a Pull Request.

## 📄 License

This project is open source and available under the MIT License.

## 📞 Support

If you encounter any issues or have feature requests, please open an issue on the [GitHub repository](https://github.com/engr-muhammad-mansoor/custom_jarunner_plugin/issues).

---

**Enjoy running your JAR files with JARunner!** ☕
