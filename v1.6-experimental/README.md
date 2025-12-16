# 🔊 Local-Text-to-Speech & Voice Input by Sid

A privacy-focused, browser-based text-to-speech and voice input application.

**Privacy Model:**
- ✅ **Text-to-Speech (TTS)**: 100% local - no data ever leaves your device
- ⚠️ **Voice Input (STT)**: Disabled by default. When enabled, may use cloud servers unless you configure offline mode on your device

[![License: GPL v3](https://img.shields.io/badge/License-GPLv3-blue.svg)](https://www.gnu.org/licenses/gpl-3.0)
[![GitHub](https://img.shields.io/badge/GitHub-sidbetatester-black.svg)](https://github.com/sidbetatester)

**Repository:** [github.com/sidbetatester/Local-text-to-speech](https://github.com/sidbetatester/Local-text-to-speech)

## ✨ Features

### 🔊 Text-to-Speech (100% Local)
- **🔒 100% Private** - All processing happens in your browser. No data leaves your device.
- **📝 Rich Text Support** - Paste from Word, Google Docs, websites - formatting preserved!
- **🎙️ Multiple Voices** - Access all voices installed on your system
- **🔍 Voice Search** - Quickly find voices by name or language
- **🌍 Language Filter** - Filter voices by language
- **⚡ Real-time Controls** - Adjust rate, pitch, and volume while speaking
- **📖 Reader View** - Follow along with word-by-word highlighting, always in sync
- **⏸️ Pause at Lines** - Natural pauses at paragraph and line breaks (toggleable)
- **📁 File Upload** - Load text from TXT, MD, HTML, CSV, JSON, XML files
- **📜 History** - Quick access to recently spoken text
- **▶️ Smart Play** - One button handles play, pause, resume, and selected text with status hints
- **⏪ Rewind/Skip** - Jump back or forward 5 words, or click any word to jump
- **⌨️ Keyboard Shortcuts** - Space to play/pause, Escape to stop, arrows to skip
- **📱 Cross-Platform** - Works on Windows, macOS, iOS, Android, ChromeOS
- **🎨 Presets** - Quick settings for Normal, Slow, Fast, Deep, and High voices
- **🔧 Formatting Toolbar** - Bold, italic, underline, lists, headings, quotes

### 🎤 Voice Input (Speech-to-Text)
- **🔒 Disabled by Default** - Must explicitly enable after reading privacy notice
- **🎤 Voice to Text** - Speak and your words appear in the editor
- **🌐 Multi-language** - Supports 12+ languages
- **📝 Continuous Mode** - Keep listening for ongoing dictation
- **✅ Can Be 100% Local** - Enable offline mode on your device (see setup guide)
- **⌨️ Quick Access** - Press M key or click 🎤 button (after enabling)
- **🏷️ Status Badge** - Shows "STT Off", "STT Cloud", or "STT Local"

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
| ▶ Play / ⏸ Pause | Smart toggle - see below |
| ⏹ Stop | Stop speaking |
| ⏪ Rewind | Jump back 5 words |
| ⏩ Forward | Skip ahead 5 words |
| 🎤 Mic | Start/stop voice input |

### Smart Play Button
The Play button intelligently handles all scenarios:

| Situation | What Happens | Status Shows |
|-----------|--------------|--------------|
| Text is selected | Speaks only the selection | `▸ Selection` |
| Currently paused | Resumes from where you paused | `Resuming` |
| Currently playing | Pauses playback | `Paused` |
| Nothing selected | Starts from the beginning | `▸ Full text` |
| Click word in Reader | Starts from that word | `▸ From word X` |

### Keyboard Shortcuts
| Key | Action |
|-----|--------|
| `Space` | Toggle Play / Pause |
| `Escape` | Stop (TTS and Voice Input) |
| `←` | Rewind 5 words |
| `→` | Skip forward 5 words |
| `M` | Toggle Voice Input |

### Voice Settings
- **Rate** - Speaking speed (0.5x to 2x)
- **Pitch** - Voice pitch (Low to High)
- **Volume** - Audio volume (0% to 100%)

### Reader View
- Switch to Reader tab to see word-by-word highlighting
- **Always in sync** - Uses word matching to stay aligned with speech
- **Formatting preserved** - bold, italic, headings, lists all display properly
- **Click any word** to jump to that position and start reading
- **Pause at lines** toggle - adds natural pauses at line/paragraph breaks
- Auto-scroll follows the current word
- Adjust font size (S/M/L/XL)

### Voice Input (Speech-to-Text)

**Privacy First:** Voice Input is disabled by default because it may send voice data to cloud servers.

**To enable:**
1. Expand the "🎤 Voice Input" section
2. Read the privacy warning
3. Choose one of:
   - **"I understand, enable Voice Input"** - Enables STT (may use cloud)
   - **"✅ I've enabled offline mode, proceed"** - Enables STT with local indicator

**After enabling:**
- Click 🎤 or press `M` to start speaking
- Your words will appear in the editor
- Badge shows: `STT Off` / `STT Cloud` / `STT Local`

**Options:**
- **Keep listening** - Continue recording after pauses (for long dictation)
- **Language** - Select from 12+ languages or auto-detect

**To disable:** Click "Disable Voice Input" at the bottom of the STT section.

**Making Voice Input 100% Local:**

By default, voice recognition may use cloud servers. To make it fully local:

| Platform | How to Enable Offline Mode |
|----------|---------------------------|
| **iOS 13+** | Settings → General → Keyboard → Enable Dictation → Enable "On-Device Dictation" |
| **macOS 12+** | System Settings → Keyboard → Dictation → Select "On-Device Only" |
| **Android** | Settings → Google → Voice → Offline Speech Recognition → Download your language |
| **Windows 11** | Settings → Privacy & Security → Speech → Turn OFF "Online speech recognition" |
| **Windows 10** | Search "Windows Speech Recognition" → Complete setup wizard |

⚠️ **Note:** Without offline mode enabled, voice data may be sent to Google (Chrome/Android) or Apple (Safari/iOS/macOS) for processing.

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

This project is licensed under the **GNU General Public License v3.0** (GPL-3.0).

This means:
- ✅ Free to use, modify, and distribute
- ✅ Attribution required - credit to [sidbetatester](https://github.com/sidbetatester)
- ✅ Derivatives must also be open source under GPL-3.0
- ✅ Commercial use allowed, but must remain open source

See [LICENSE](LICENSE) file or [gnu.org/licenses/gpl-3.0](https://www.gnu.org/licenses/gpl-3.0) for details.

**Copyright © 2025 Sid ([@sidbetatester](https://github.com/sidbetatester))**

## 🤝 Contributing

Contributions are welcome! Feel free to:
- Report bugs
- Suggest features
- Submit pull requests

## 📋 Changelog

### v1.3.2
- **Privacy First**: Voice Input (STT) now disabled by default
- Added: Privacy warning that must be acknowledged before enabling STT
- Added: Two enable options - "I understand" (cloud) or "I've enabled offline mode" (local)
- Added: Clear badge indicators showing STT status (Off / Cloud / Local)
- Added: "Disable Voice Input" button to turn it off after enabling
- Added: STT state saved to localStorage (persists between sessions)
- Improved: M keyboard shortcut opens STT section if not enabled

### v1.3.1
- Improved: Voice dropdown now shows language/locale (e.g., "English (US)", "English (UK)")
- Improved: Voice info display shows locale, quality rating, and if it's local or network
- Improved: Language filter shows readable names with voice counts
- Improved: Voice search now searches locale names too (try "british" or "australia")
- Added: 🔄 Refresh button to reload voices if some are missing
- Added: More retry attempts for loading voices on Apple devices
- Fixed: No-speech error now continues listening instead of stopping

### v1.3.0
- Added: Voice Input (Speech-to-Text) feature
- Added: 🎤 button to start/stop voice input
- Added: M keyboard shortcut for voice input
- Added: Continuous mode for ongoing dictation
- Added: Multi-language support (12+ languages)
- Added: Detailed setup guide for offline voice recognition on all platforms
- Added: Interim results display while speaking

### v1.2.6
- Improved: Word sync now uses word content matching instead of character position
- Fixed: Handles special characters like parentheses, underscores in code snippets
- Fixed: Self-corrects when sync drifts by matching spoken word to display word
- Fixed: Works correctly when starting from middle of text

### v1.2.5
- Fixed: Word highlighting stays in sync using character position mapping
- Fixed: Clicking words in Reader view now correctly starts from that word
- Both fixes work together - click any word and highlighting tracks accurately

### v1.2.4
- Fixed: Word highlighting now stays in sync by matching actual spoken words
- Uses word content matching instead of character position (more reliable)
- Handles preprocessed text (pauses) without losing sync

### v1.2.3
- Fixed: Now reads numbered list items with their numbers (1, 2, 3...)
- Fixed: Bullet points are read as "bullet" marker
- Reader view shows the numbers/bullets as they'll be spoken

### v1.2.2
- Added "Pause at lines" toggle - speech now pauses naturally at paragraph/line breaks
- Setting is saved and persists across sessions

### v1.2.1
- Reader view now preserves formatting (bold, italic, headings, lists, etc.)
- Word highlighting works within formatted text

### v1.2.0
- Smart Play button - handles play, pause, resume, and selected text automatically
- **Selection takes priority** - if text is selected, Play reads the selection first
- Status hints show what's being read: `▸ Full text`, `▸ Selection`, `▸ From word X`
- Removed separate Selection button - Play does it all
- Added rewind (⏪) and skip forward (⏩) buttons - jumps 5 words
- Added keyboard shortcuts: ← rewind, → skip forward
- Click any word in Reader view to jump to that position
- Words in Reader view now highlight on hover

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
