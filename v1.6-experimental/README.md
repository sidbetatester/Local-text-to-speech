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
# 🔊 Local-Text-to-Speech & Voice Input — v1.6-experimental

Privacy-first, single-file browser TTS + optional local STT (experimental).

**Quick privacy summary:**
- ✅ TTS (speechSynthesis) is fully local — audio is generated by your device
- ⚠️ STT (SpeechRecognition) is disabled by default and may be cloud-backed unless you enable on-device/offline speech on your platform

[![License: GPL v3](https://img.shields.io/badge/License-GPLv3-blue.svg)](https://www.gnu.org/licenses/gpl-3.0)

## What's new in v1.6-experimental
- Inline input sanitizer (compact DOMPurify-like implementation) — sanitizes pasted or loaded HTML before insertion
- Optional local encryption of stored data using Web Crypto (PBKDF2 → AES-GCM)
- Passphrase modal to enable/unlock encryption and a status badge showing encryption state
- Encrypted storage layout: `enc_meta` (metadata) + per-item blobs at keys prefixed with `enc:` (e.g. `enc:ttsHistory`)
- Migration: when enabling encryption plaintext keys are migrated into `enc:` blobs and plaintext keys removed
- Wipe-on-exit now fully resets the app, including deleting `enc_meta` and all `enc:` blobs
- Manual "Reset encryption (delete all encrypted data)" action available from the lock icon modal
- Single-file distribution — no remote dependencies; CSP deployment story provided below

## Important Security & Recovery Notes
- Passphrase is the only way to decrypt your encrypted data. If you forget it, data is unrecoverable.
- Clearing browser storage or uninstalling the browser may remove encrypted blobs and make them unrecoverable.
- Wipe-on-exit will delete all encrypted data if enabled (destructive by design).
- Async operations during `beforeunload`/`pagehide` are unreliable across browsers — the app attempts to clear data but this cannot be guaranteed in all environments.

## How encryption works (brief)
- Derivation: PBKDF2 with SHA-256 and a per-install salt stored in `enc_meta` (iterations are configurable at enable time)
- Cipher: AES-GCM 256-bit, unique IV per encrypted blob
- Storage: encrypted JSON blobs are base64-encoded and saved under `enc:<key>`; `enc_meta` stores salt, version, and iteration count
- Runtime: the derived `masterKey` is kept in-memory only; locking or clearing the page clears it

## Developer notes (storage keys & migration)
- `enc_meta` — contains salt (base64), iterations, and version
- Encrypted blobs: keys of the form `enc:<originalKey>` (e.g. `enc:ttsHistory`, `enc:ttsSettings`)
- On enable: plaintext keys are migrated → `enc:<key>` blobs, then plaintext keys removed
- To completely reset encryption call the app's Reset action which removes `enc_meta` and all `enc:` keys

## Backup / Export (recommended)
- v1.6 does not include a GUI export/import yet — strongly recommended to implement before relying on encrypted storage for important data
- Backup approach: export `enc_meta` plus all `enc:` blobs (exact key list) into a single file. Restore by importing and placing them back into localStorage.

## CSP deployment story
- This distribution is single-file and contains inline scripts/styles. For strict CSP you can compute the SHA-256 hash of the final, frozen `index.html` script block and use it in `script-src 'sha256-<hash>'`.
- Note: the hash must match the exact file bytes. Compute the hash after you freeze the file.

## UI & UX
- Encryption unlock/enable modal reachable from the lock icon. Options include enabling encryption (create passphrase) and unlocking with an existing passphrase.
- Reset encryption button appears in the modal when `enc_meta` exists — it asks for confirmation before deleting encrypted data.
- Private Mode toggle prevents storing transcripts and limits history persistence.

## Limitations & Recommendations
- Passphrase loss is catastrophic — provide export/import backups to recover data.
- PBKDF2 iterations: high iterations increase security but may be slow on low-end devices; consider adding a progress indicator or WebWorker offload.
- Relying on `beforeunload`/`pagehide` for destructive wipes is best-effort; do not assume absolute guarantees across browsers.

## Remaining priorities (suggested)
1. Add Export / Import encrypted backup UI (high priority)
2. Add PBKDF2 progress indicator or move key derivation to a WebWorker
3. Freeze final file and compute script SHA‑256 for CSP

## Changelog (high level)
### v1.6-experimental
- Added: inline sanitizer, encrypted localStorage (Web Crypto), passphrase modal
- Added: `enc_meta` + `enc:` storage format, migration from plaintext
- Changed: `clearSensitiveData()` wipes both plaintext and encrypted blobs; wipe-on-exit is destructive when enabled
- Added: Reset button to delete all encrypted data

---

Made with ❤️ by [Sid](https://github.com/sidbetatester) privacy-first local TTS experimental build
