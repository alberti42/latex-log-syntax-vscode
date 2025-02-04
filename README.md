# LaTeX Log Syntax Highlighting for VS Code

This VS Code extension provides syntax highlighting for LaTeX log files using the **TextMate** grammar format. It is based on the syntax definition from the official [TextMate LaTeX Bundle](https://github.com/textmate/latex.tmbundle), specifically the LaTeX log syntax file found [here](https://raw.githubusercontent.com/textmate/latex.tmbundle/refs/heads/master/Syntaxes/LaTeX%20Log.plist).

## Features

- **Syntax Highlighting**: LaTeX log files will now have proper syntax highlighting for various LaTeX-related log elements such as:
  - Errors
  - Warnings
  - Info messages
  - Comments
  - LaTeX commands
  - Block elements
  
- **Based on TextMate Grammar**: This extension uses the TextMate grammar format, which provides an efficient and consistent way to highlight LaTeX log files.

## Installation

To install this extension:

1. **Clone the repository** or download it as a ZIP file.
2. Open **VS Code** and navigate to the **Extensions** panel.
3. Click the **...** button and select **"Install from VSIX..."**.
4. Select the `.vsix` file you have downloaded and installed it.

Alternatively, you can also install the extension by directly using the `.tmLanguage` files or building a `.vsix` package.

## Syntax Supported

This extension recognizes and highlights the following syntax patterns:

- **Errors**: Highlight `Error:` messages with distinct coloring.
- **Warnings**: `Warning:` and `Overfull`/`Underfull` messages are highlighted.
- **Info**: `Info:` messages receive different highlighting.
- **Commands**: LaTeX commands are clearly identified.
- **Comments**: Comments within LaTeX logs are colored accordingly.

## Files in the Repository

- **`package.json`**: Contains metadata and configuration for the VS Code extension.
- **`syntaxes/LaTeXLog.tmLanguage`**: The TextMate grammar for LaTeX log files, converted from the original `.plist`.
- **`syntaxes/LaTeXLog.tmLanguage.json`**: A JSON version of the TextMate grammar for compatibility with VS Code.
- **`syntaxes/LaTeXLog.yaml`**: A YAML-based alternative for syntax definition.

## Usage

Once the extension is installed, any LaTeX log file (typically with the `.log` extension) will be automatically associated with the LaTeX Log syntax, providing syntax highlighting throughout the file.

You can also configure file associations for `.log` files in your settings:

```json
"files.associations": {
  "*.log": "latex-log"
}
```

## License

This project is licensed under the MIT License. See the LICENSE file for details.

## Acknowledgements

This extension borrows its syntax highlighting rules from the TextMate LaTeX Bundle. Special thanks to the TextMate community for providing the initial syntax grammar.

When you copy this into your `README.md` file, it will show as raw Markdown text and preserve the formatting and code fences as requested.

