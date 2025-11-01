# Share to PDF

[![Vibe Coded](https://img.shields.io/badge/🎵_Vibe-Coded-blueviolet?style=for-the-badge)](https://github.com/bodfather/obsidian-share-pdf#-vibe-coded--ai-assisted-development)
[![AI-Assisted Development](https://img.shields.io/badge/AI-Assisted_Development-00D4FF?style=for-the-badge&logo=anthropic)](https://www.anthropic.com/claude)
[![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg?style=for-the-badge)](https://opensource.org/licenses/MIT)

Convert and save your Obsidian notes as beautifully formatted PDFs with full support for markdown formatting, images, and code blocks. Works seamlessly on desktop and mobile devices.

## Features

- **Complete Markdown Support**: Bold, italic, headings, lists, blockquotes, code blocks, and more
- **Image Handling**: Embedded images with automatic base64 conversion
- **Theme Integration**: Automatically matches your Obsidian theme colors
- **Custom Styling**: Configure fonts, sizes, margins, and spacing
- **Smart Page Breaks**: Avoid awkward splits in content
- **Mobile Sharing**: Native share functionality on Android and iOS
- **Overwrite Protection**: Optional confirmation before replacing existing PDFs
- **Customizable Output**: Control PDF location, paper size, and margins

## Installation

### From Obsidian Community Plugins

1. Open Obsidian Settings
2. Navigate to **Community Plugins** and disable Safe Mode
3. Click **Browse** and search for "Share to PDF"
4. Click **Install**, then **Enable**

### Manual Installation

1. Download the latest release from the [GitHub releases page](https://github.com/bodfather/obsidian-share-pdf)
2. Extract the files to your vault's plugins folder: `<vault>/.obsidian/plugins/share-to-pdf/`
3. Reload Obsidian
4. Enable the plugin in Settings → Community Plugins

## Usage

### Basic Usage

1. Open any note you want to convert to PDF
2. Use the command palette (Ctrl/Cmd + P) and search for "Share to PDF"
3. Or use the ribbon icon (if enabled in settings)
4. The PDF will be saved to your configured output folder

### Mobile Usage

On mobile devices, after the PDF is saved, the native share dialog will automatically appear, allowing you to:
- Share via email, messaging apps, or other installed apps
- Save to cloud storage
- Send to nearby devices
- Print directly

## Settings

### Output Settings

- **PDF Output Folder**: Choose where PDFs are saved (default: `PDFs`)
- **Warn before overwriting**: Show confirmation dialog before replacing existing PDF files

### Page Settings

- **Paper Size**: A4 or Letter
- **Orientation**: Portrait or Landscape
- **Margin Size**: Top, bottom, left, and right margins in mm

### Typography

- **Font Family**: Choose from serif, sans-serif, or monospace
- **Font Size**: Base font size for body text (default: 12pt)
- **Line Height**: Space between lines for better readability

### Styling

- **Code Block Background**: Background color for code blocks
- **Link Color**: Color for hyperlinks in the PDF
- **Heading Styles**: Customize size and weight for each heading level
- **Use Theme Colors**: Automatically apply your Obsidian theme colors

### Content Options

- **Include Metadata**: Add frontmatter data to the PDF header
- **Show Page Numbers**: Display page numbers at the bottom
- **Smart Page Breaks**: Prevent awkward content splits across pages

## Supported Markdown Features

### Text Formatting
- **Bold** text with `**bold**` or `__bold__`
- *Italic* text with `*italic*` or `_italic_`
- `Inline code` with backticks
- ~~Strikethrough~~ with `~~text~~`

### Headings
All heading levels (H1-H6) with customizable styling

### Lists
- Unordered lists with `-`, `*`, or `+`
- Ordered lists with numbers
- Nested lists with proper indentation
- Task lists with `- [ ]` and `- [x]`

### Blockquotes
> Blockquotes with `>` prefix
> Can span multiple lines

### Code Blocks
```javascript
// Syntax highlighting with language tags
function example() {
  return true;
}
```

### Links and Images
- `[Link text](url)` for hyperlinks
- `![Alt text](image.png)` for images
- Internal wiki-links `[[Note Name]]`

### Horizontal Rules
Dividers with `---` or `***`

### Tables
| Feature | Supported |
|---------|-----------|
| Tables  | Yes       |
| Alignment | Yes     |

## Development

### Building from Source

```bash
# Clone the repository
git clone https://github.com/bodfather/obsidian-share-pdf.git
cd obsidian-share-pdf

# Install dependencies
npm install

# Build the plugin
npm run build

# Or run in development mode with auto-rebuild
npm run dev
```

### Project Structure

```
obsidian-share-pdf/
├── main.js           # Compiled plugin code
├── manifest.json     # Plugin metadata
├── styles.css        # Plugin styles
├── esbuild.config.mjs # Build configuration
└── README.md         # This file
```

## Troubleshooting

### PDFs are not saving
- Check that the output folder path is valid
- Ensure you have write permissions in your vault
- Try creating the output folder manually

### Images are missing in PDF
- Verify images exist in your vault
- Check that image paths are correct
- Supported formats: PNG, JPEG, GIF, SVG

### Formatting looks wrong
- Try toggling "Use Theme Colors" setting
- Adjust font size and line height
- Check if custom CSS is interfering

### Mobile share not working
- Ensure you're running on a mobile device
- Check that your OS supports the share API
- Try updating your Obsidian app

## 🎵 Vibe Coded | AI-Assisted Development

This plugin was developed through **AI-assisted programming** - a collaborative process between human direction and AI implementation.

**The Development Process:**

👨‍💻 **Human (bodfather)**
- Product vision and feature requirements
- UX decisions and design direction
- Testing, debugging, and quality assurance
- Architecture decisions and technical approach

🤖 **AI Assistant (Claude)**
- Code implementation and generation
- PDF generation logic and jsPDF integration
- Theme color extraction and parsing
- Documentation and README creation

**Transparency Commitment:**

We believe in being honest about development processes. This plugin was built using Claude AI assistance, and we're proud of it! AI-assisted development is the future of software creation.

**Want to build your own vibe-coded project?**

Add this badge to your README:

```markdown
[![Vibe Coded](https://img.shields.io/badge/🎵_Vibe-Coded-blueviolet?style=for-the-badge)](https://github.com/bodfather/obsidian-share-pdf#-vibe-coded--ai-assisted-development)
```

---

## Credits

- Built with [jsPDF](https://github.com/parallax/jsPDF) for PDF generation
- Uses Obsidian Plugin API
- Developed in collaboration with Claude AI
- Inspired by the need for better mobile PDF sharing

## License

MIT License - see [LICENSE](LICENSE) file for details

## Support

- Report issues on [GitHub](https://github.com/bodfather/obsidian-share-pdf/issues)
- For general questions, visit the [Obsidian forum](https://forum.obsidian.md/)

## Changelog

### 1.0.0 (Initial Release)
- Complete markdown to PDF conversion
- Theme color integration
- Mobile sharing support
- Customizable page settings
- Typography controls
- Overwrite protection
- Image embedding
- Code block syntax highlighting
- Table support
- Smart page breaks
