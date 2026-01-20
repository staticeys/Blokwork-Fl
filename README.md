# Blokwork Fl Web Edition

**A privacy-focused, offline-first notes app that runs entirely in your browser.**

[Launch App](https://staticeys.github.io/Blokwork-Fl/)

## What is Blokwork?

Blokwork is a note-taking / text block management app built with Flutter. It helps you capture, organise, and manage blocks of text. It features markdown support, tagging, sorting and export capabilities.

**This web version runs completely in your browser** - no servers, no cloud sync, no data collection. Your notes stay on your device.

---

## ✨ Features

### 📝 Block-Based Note Taking
- Create unlimited plain text notes as individual "blocks"
- Add reference links 
- Full **GitHub Flavored Markdown**
- Right click blocks to access the context menu, manage metadata and copy blocks as rich text

### 🏷️ Organization & Filtering
- **Tag blocks** with custom colored labels
- Filter blocks by multiple tags
- Search across all blocks
- Sort by creation or modification date
- Workspace-based organization

### 🎨 Beautiful Theming
- **Light, Dark, and Monochrome** themes
- Multiple color scheme presets
- Customizable accent colors
- Material Design 3 components

### 💾 Import & Export
- **Export to JSON** - Full workspace backup
- **Export to CSV** - Spreadsheet-compatible format
- **Export to Markdown** - ZIP archive of .md files
- **Import from JSON** - Restore complete workspaces
- **Import from CSV** - Bulk import with column mapping

### 🗂️ Workspace Management
- Create multiple workspaces
- Switch between workspaces instantly
- Rename and organize workspaces
- Each workspace has independent blocks and tags

### 🔒 Privacy-First Design
- **100% offline** - Works without internet after initial load
- **Local storage only** - Data never leaves your browser
- **No tracking or analytics** - Zero telemetry
- **No external dependencies** - All resources bundled locally
- **No accounts required** - Start using immediately

---

## 🚀 Getting Started

### First Launch

1. **Visit the app** - Open in any modern browser
2. **Create a workspace** - Give it a name (e.g., "Personal Notes")
3. **Create your first block** - Click the + button to add a note
4. **Write in markdown** - Use the toolbar or type markdown syntax
5. **Organise with tags** - Right click to create tags and assign them to blocks

### Tips for New Users

- **Markdown basics**: Use `#` for headings, `**bold**`, `*italic*`, `` `code` ``
- **Quick search**: Start typing in the search bar to filter blocks
- **Theme switching**: Visit Settings to change between light/dark themes
- **Backup regularly**: Export your workspace as JSON for safe keeping

---

## 🔐 Security & Privacy

### Data Storage

Your data is stored using your browser's **localStorage** API:
- **Location**: Stored locally on your device only
- **Persistence**: Data survives browser restarts
- **Size limit**: Typically 5-10MB per domain (varies by browser)
- **Clearing data**: Use browser settings or workspace deletion

### No Network Activity

After the initial page load, Blokwork makes **zero network requests**:
- ✅ No API calls to external servers
- ✅ No font loading from CDNs (uses system fonts)
- ✅ No analytics or tracking pixels
- ✅ No third-party scripts
- ✅ Works completely offline

### Content Security Policy

Strict CSP headers prevent:
- Cross-site scripting (XSS) attacks
- Unauthorized data exfiltration
- Third-party script injection
- Clickjacking attempts

View the CSP in action: Right-click → Inspect → Console

### Open Source & Auditable

- **Source code**: Publicly available on GitHub
- **Build process**: Reproducible Flutter web builds
- **Dependencies**: All listed in pubspec.yaml
- **No obfuscation**: Readable code for community review

---

## 🌐 Browser Compatibility

### Recommended Browsers

| Browser | Version | Status |
|---------|---------|--------|
| Chrome/Edge | 100+ | ✅ Fully supported |
| Firefox | 100+ | ✅ Fully supported |
| Safari | 15+ | ✅ Fully supported |
| Mobile browsers | ...not great

---

## 📊 Technical Details

### Technology Stack

- **Framework**: Flutter 3.3+ (compiled to JavaScript)
- **Rendering**: CanvasKit renderer for high-fidelity UI
- **State Management**: Riverpod
- **Storage**: Browser localStorage API
- **Markdown**: markdown_widget + flutter_highlight
- **No backend**: Pure client-side application

### Performance

- **Initial load**: ~2-5 seconds (depending on connection)
- **Runtime**: Smooth
- **Memory**: ~50-100MB typical usage
- **Storage**: ~10KB per workspace + blocks

### Offline Capabilities

Once loaded, the app is **fully functional offline**:
- ✅ Create and edit blocks
- ✅ Manage tags and workspaces
- ✅ Change themes
- ✅ Export data (downloads work offline)
- ❌ Initial page load (requires internet once)
- ❌ Import files (browser file picker requires connection)

---

## 💡 Use Cases

### Perfect For

- 📚 **Personal knowledge base** - Organize research and notes
- ✍️ **Writing drafts** - Compose blog posts or articles
- 📋 **Meeting notes** - Quick capture with tags
- 💻 **Code snippets** - Store with syntax highlighting
- 🎓 **Study notes** - Tag by subject or topic
- 🗂️ **Project planning** - Track ideas and todos

### Not Ideal For

- ❌ **Collaboration** - Single-user, local-only
- ❌ **Mobile-primary usage** - Desktop-optimized UI
- ❌ **Large media files** - Text-focused, no attachments on web
- ❌ **Cross-device sync** - No cloud sync (export/import instead)

---

## 📥 Backup & Data Portability

### Recommended Backup Strategy

1. **Regular exports**: Download JSON backup weekly
2. **Version control**: Keep previous exports
3. **Multiple locations**: Store backups in cloud storage (encrypted)
4. **Test restores**: Periodically verify imports work

---

## ⚠️ Important Notes

### Data Persistence

- **Browser data** can be cleared if you:
  - Clear browsing data/history
  - Use incognito/private mode
  - Reinstall browser
  - Use browser cleanup tools
- **Always export** important workspaces as JSON backups

### Storage Limits

- Most browsers allow **5-10MB** of localStorage
- A workspace with 1,000 blocks typically uses ~2MB
- Monitor your usage and export large workspaces
- Browser will warn if quota is exceeded

### Browser Updates

- Keep your browser updated for security
- Test after major browser updates
- Report compatibility issues on GitHub

---

## 🐛 Troubleshooting

### Text Not Displaying

If text appears blank after loading:
1. Hard refresh: `Ctrl+F5` (Windows) or `Cmd+Shift+R` (Mac)
2. Clear browser cache
3. Check browser console for CSP errors
4. Try a different browser

### App Won't Load

1. Check internet connection (required for first load)
2. Disable browser extensions temporarily
3. Try incognito/private mode
4. Clear site data and reload

### Data Lost

1. Check if you switched workspaces accidentally
2. Try different browser (data is browser-specific)
3. Restore from last JSON export
4. Contact support with details

### Performance Issues

1. Export and archive old workspaces
2. Reduce blocks per workspace (<500 recommended)
3. Close unnecessary browser tabs
4. Use a Chromium-based browser for best performance

---

## 📞 Support & Feedback

### Get Help

- **Documentation**: See main [README.md](https://github.com/yourusername/blokwork)
- **Bug reports**: [GitHub Issues](https://github.com/yourusername/blokwork/issues)
- **Feature requests**: [GitHub Discussions](https://github.com/yourusername/blokwork/discussions)

### Contributing

Blokwork is open source! Contributions welcome:
- Report bugs and issues
- Suggest features
- Submit pull requests
- Improve documentation

---

## 📜 License

MIT License - See [LICENSE](../LICENSE) file for details.

**You are free to:**
- ✅ Use for personal or commercial purposes
- ✅ Modify and redistribute
- ✅ Self-host on your own domain

---

## 🙏 Acknowledgments

Built with Flutter and powered by open source:
- [Flutter](https://flutter.dev) - UI framework
- [Riverpod](https://riverpod.dev) - State management
- [markdown_widget](https://pub.dev/packages/markdown_widget) - Markdown rendering
- [And many more](../pubspec.yaml) - See full dependency list

---

**Enjoy distraction-free, privacy-focused note-taking!** 🚀

*Last updated: 2025-12-18*
