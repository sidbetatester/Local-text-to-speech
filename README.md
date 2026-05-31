# 🔊 Local-Text-to-Speech by Sid

A privacy-focused, browser-based text-to-speech application that runs 100% locally on your device. No data is ever sent to external servers.

[![License: Source Available](https://img.shields.io/badge/License-Source--Available-orange.svg)](LICENSE)
[![GitHub](https://img.shields.io/badge/GitHub-sidbetatester-black.svg)](https://github.com/sidbetatester)

**Repository:** [github.com/sidbetatester/Local-text-to-speech](https://github.com/sidbetatester/Local-text-to-speech)

## ✨ Features

- **🔒 100% Private** - All processing happens in your browser. No data leaves your device.
- **📝 Rich Text Support** - Paste from Word, Google Docs, websites - formatting preserved!
- **🎙️ Multiple Voices** - Access all voices installed on your system
- **🔍 Voice Search** - Quickly find voices by name or language
- **🌍 Language Filter** - Filter voices by language
- **⚡ Real-time Controls** - Adjust rate, pitch, and volume while speaking
- **📖 Reader View** - Follow along with word-by-word highlighting
- **📁 File Upload** - Load text from TXT, MD, HTML, CSV, JSON, XML files
- **📜 History** - Quick access to recently spoken text
- **⌨️ Keyboard Shortcuts** - Space to play/pause, Escape to stop
- **📱 Cross-Platform** - Works on Windows, macOS, iOS, Android, ChromeOS
- **🎨 Presets** - Quick settings for Normal, Slow, Fast, Deep, and High voices
- **🔧 Formatting Toolbar** - Bold, italic, underline, lists, headings, quotes

## 🚀 Quick Start

### Option 1: Direct Use
1. Download `text-to-speech.html`
2. Open it in any modern browser
3. Start typing or paste text
4. Click Play

### Option 2: Host Online
See [Hosting](#-hosting) section below.

## 🎮 Usage

### Basic Controls
| Control | Action |
|---------|--------|
| ▶ Play | Start speaking |
| ⏸ Pause | Pause/resume speech |
| ⏹ Stop | Stop speaking |
| ✂ Selection | Speak selected text only |

### Keyboard Shortcuts
| Key | Action |
|-----|--------|
| `Space` | Play / Pause |
| `Escape` | Stop |

### Voice Settings
- **Rate** - Speaking speed (0.5x to 2x)
- **Pitch** - Voice pitch (Low to High)
- **Volume** - Audio volume (0% to 100%)

### Reader View
- Switch to Reader tab to see word-by-word highlighting
- Auto-scroll follows the current word
- Adjust font size (S/M/L/XL)

### Rich Text Support
The editor preserves formatting when you paste from:
- Microsoft Word
- Google Docs
- Web pages
- Emails
- PDF (copy/paste)

**Preserved formatting:**
- Bold, italic, underline
- Headings (H1, H2, H3)
- Bullet and numbered lists
- Blockquotes
- Links (displayed, not clickable in TTS)

**Toolbar buttons:**
| Button | Function |
|--------|----------|
| **B** | Bold |
| *I* | Italic |
| U̲ | Underline |
| • | Bullet list |
| 1. | Numbered list |
| H | Heading |
| " | Blockquote |
| ✕ | Clear formatting |

**Plain Text Mode:** Click "Plain Text" button to strip formatting when pasting.

### File Upload
Supported formats:
- `.txt` - Plain text
- `.md` - Markdown
- `.html` - HTML (tags stripped)
- `.csv` - CSV data
- `.json` - JSON files
- `.xml` - XML files

Maximum file size: 5MB

## 🌐 Hosting

### Netlify (Easiest)
1. Go to [app.netlify.com/drop](https://app.netlify.com/drop)
2. Drag and drop `text-to-speech.html`
3. Done! You get an instant HTTPS URL

### GitHub Pages (Recommended for Permanent Hosting)
1. Create a new GitHub repository
2. Upload `text-to-speech.html` as `index.html`
3. Go to Settings → Pages
4. Select "Deploy from a branch" → main
5. Your site will be live at `https://yourusername.github.io/repo-name`

### Other Free Options
- Vercel
- Cloudflare Pages
- Render
- Surge.sh

## 🔐 Privacy & Security

### Data Privacy
- ✅ No data collection
- ✅ No analytics or tracking
- ✅ No external API calls
- ✅ No cookies (except localStorage for settings)
- ✅ All processing is local to your browser

### Security
- ✅ No external scripts or dependencies
- ✅ XSS protected (all input is sanitized)
- ✅ No database or server-side code
- ✅ Safe to host publicly

### What's Stored Locally
The app uses browser localStorage to save:
- Voice preference
- Rate, pitch, volume settings
- Recent history (last 15 items)

This data never leaves your device and can be cleared anytime.

## 🖥️ Browser Compatibility

| Browser | Support |
|---------|---------|
| Chrome | ✅ Full |
| Edge | ✅ Full |
| Safari | ✅ Full |
| Firefox | ✅ Full |
| Opera | ✅ Full |
| iOS Safari | ✅ Full (with minor limitations) |
| Android Chrome | ✅ Full |

### Platform Notes
- **Windows** - Best voice selection with installed TTS voices
- **macOS** - High-quality system voices available
- **iOS** - Works well; pause/resume may be slightly unreliable
- **Android** - Works with device voices

## 💡 Tips for Better Voices

### Windows
Settings → Time & Language → Speech → Add voices

### macOS
System Settings → Accessibility → Spoken Content → System Voice → Manage Voices

### iOS
Settings → Accessibility → Spoken Content → Voices

### Android
Settings → Accessibility → Text-to-speech output

## 📝 License

This project is licensed under the **Local-Text-to-Speech Source-Available License v1.0**.

This means:
- Source code is available to view and study.
- Personal, non-commercial use of unmodified copies is allowed.
- Modification, redistribution, public hosting, and commercial use require prior written permission.
- Attribution and license notices must be preserved.

See the [LICENSE](LICENSE) file for details.

**Copyright © 2025 Sid ([@sidbetatester](https://github.com/sidbetatester))**

## 🤝 Contributing

Contributions are welcome! Feel free to:
- Report bugs
- Suggest features
- Submit pull requests

## 📋 Changelog

### v1.1.0
- Added rich text editor with formatting toolbar
- Paste from Word, Google Docs, websites with formatting preserved
- Bold, italic, underline, headings, lists, blockquotes support
- Plain text mode toggle
- Improved Markdown file parsing
- HTML file formatting preserved on upload

### v1.0.0
- Initial release
- Multi-voice support with search and filtering
- Real-time playback controls
- Reader view with word highlighting
- File upload support
- History management
- Keyboard shortcuts
- Cross-platform compatibility

---

Made with ❤️ by [Sid](https://github.com/sidbetatester) for privacy-conscious users
