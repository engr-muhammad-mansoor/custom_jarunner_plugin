# JARunner - VS Code Extension

A lightweight Visual Studio Code extension that allows you to quickly run JAR files directly from your workspace with a simple keyboard shortcut.

## 🚀 Features

- **Quick JAR Execution**: Run JAR files instantly with a keyboard shortcut
- **Integrated Terminal**: Automatically opens a dedicated terminal for JAR execution
- **Cross-Platform**: Works on Windows, macOS, and Linux
- **Simple Configuration**: Easy to set up and use

## 📋 Requirements

- **Visual Studio Code**: Version 1.85.0 or higher
- **Java Runtime Environment (JRE)**: Must be installed and accessible via command line
- **Node.js**: Required for development/build purposes

## 🔧 Installation

### From VS Code Marketplace (Coming Soon)
1. Open VS Code
2. Go to Extensions view (`Ctrl+Shift+X` / `Cmd+Shift+X`)
3. Search for "JARunner"
4. Click Install

### Manual Installation
1. Clone this repository:
   ```bash
   git clone https://github.com/engr-muhammad-mansoor/custom_jarunner_plugin.git
   cd custom_jarunner_plugin
   ```

2. Install dependencies:
   ```bash
   npm install
   ```

3. Compile the extension:
   ```bash
   npm run compile
   ```

4. Press `F5` to open a new Extension Development Host window
5. In the new window, use the extension command

## 📖 Usage

### Running a JAR File

1. **Using Keyboard Shortcut**:
   - Press `Ctrl+Alt+J` (Windows/Linux) or `Cmd+Alt+J` (macOS)
   - The extension will execute the configured JAR file in a new terminal

2. **Using Command Palette**:
   - Press `Ctrl+Shift+P` (Windows/Linux) or `Cmd+Shift+P` (macOS)
   - Type "JarFileRun" and select the command
   - The JAR file will execute in a dedicated terminal

### Configuration

Before using the extension, you'll need to update the JAR file path in `src/extension.ts`:

```typescript
const command = `java -jar "${'path/to/your/jarfile.jar'}"`;
```

Replace `path/to/your/jarfile.jar` with the actual path to your JAR file.

**Future Enhancement**: This extension will be updated to support file picker for selecting JAR files dynamically.

## 🛠️ Development

### Project Structure

```
custom_jarunner_plugin/
├── src/
│   ├── extension.ts      # Main extension code
│   └── test/
│       └── extension.test.ts
├── out/                  # Compiled JavaScript files
├── package.json          # Extension manifest
├── tsconfig.json         # TypeScript configuration
└── README.md
```

### Build Commands

- `npm run compile` - Compile TypeScript to JavaScript
- `npm run watch` - Watch for changes and recompile
- `npm run lint` - Run ESLint
- `npm test` - Run tests
- `npm run vscode:prepublish` - Prepare extension for publishing

### Debugging

1. Open the project in VS Code
2. Press `F5` to launch the Extension Development Host
3. Use the Command Palette to test the extension

## 📝 Extension Settings

Currently, this extension does not contribute any VS Code settings. The JAR file path is configured directly in the source code.

## 🤝 Contributing

Contributions are welcome! Please feel free to submit a Pull Request.

1. Fork the repository
2. Create your feature branch (`git checkout -b feature/AmazingFeature`)
3. Commit your changes (`git commit -m 'Add some AmazingFeature'`)
4. Push to the branch (`git push origin feature/AmazingFeature`)
5. Open a Pull Request

## 📄 License

This project is open source and available under the [MIT License](LICENSE).

## 🙏 Acknowledgments

- Built with [VS Code Extension API](https://code.visualstudio.com/api)
- TypeScript for type-safe development

## 🐛 Known Issues

- JAR file path is currently hardcoded and needs to be manually updated in the source code
- Future versions will include a file picker for dynamic JAR file selection

## 📞 Support

If you encounter any issues or have feature requests, please open an issue on the [GitHub repository](https://github.com/engr-muhammad-mansoor/custom_jarunner_plugin/issues).

---

**Enjoy running your JAR files with JARunner!** ☕
