# Chrome Memory Tracker

[![Build](https://github.com/eswar06/chrome-memory-tracker/actions/workflows/build.yml/badge.svg)](https://github.com/eswar06/chrome-memory-tracker/actions/workflows/build.yml)
[![Lint](https://github.com/eswar06/chrome-memory-tracker/actions/workflows/lint.yml/badge.svg)](https://github.com/eswar06/chrome-memory-tracker/actions/workflows/lint.yml)
[![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](LICENSE)
[![TypeScript](https://img.shields.io/badge/TypeScript-5.9-blue)](https://www.typescriptlang.org/)
[![React](https://img.shields.io/badge/React-19.2-blue)](https://react.dev/)

A Chrome Extension (Manifest V3) built with React + TypeScript that tracks browsing time and captures user highlights using the Chrome Extensions API.

> A productivity tool for personal knowledge management and memory capture.

## 📋 Overview

This project demonstrates:

- Manifest V3 architecture and best practices
- Background service workers for efficient resource usage
- Content scripts for user interaction capture
- chrome.storage.local for persistent local storage
- React-based popup UI with TypeScript
- Type-safe state management

## ✨ Features

- **Track Time Spent** - Monitor browsing time per page
- **Capture Highlights** - Save selected text via context menu
- **Local Storage** - Persistent storage, no backend required
- **Search Functionality** - Quickly find saved entries
- **Toggle Tracking** - Enable/disable tracking on demand
- **Clear Memory** - Manage stored data easily

## 🛠 Tech Stack

| Technology | Version | Purpose |
|-----------|---------|---------|
| React | ^19.2.0 | UI Framework |
| TypeScript | ^5.9.3 | Type Safety |
| Vite | 7.2.5 | Build Tool |
| Chrome API | Manifest V3 | Extension API |
| ESLint | ^9.39.1 | Code Quality |

## 🏗 Architecture

```
src/
├── background.ts       → Handles tab events + time tracking
├── content.ts          → Captures selected text
├── popup/              → React-based UI components
├── storage.ts          → Storage abstraction layer
└── types/              → TypeScript type definitions
```

## 🚀 Installation (Development)

### Prerequisites
- Node.js 20+
- Chrome/Chromium browser
- npm or yarn

### Setup Steps

1. **Clone the repository**
   ```bash
   git clone https://github.com/eswar06/chrome-memory-tracker.git
   cd chrome-memory-tracker
   ```

2. **Install dependencies**
   ```bash
   npm install
   ```

3. **Build the extension**
   ```bash
   npm run build
   ```

4. **Load in Chrome**
   - Open Chrome and navigate to `chrome://extensions`
   - Enable "Developer Mode" (toggle in top right)
   - Click "Load unpacked"
   - Select the `dist/` folder from this project

5. **Start development (optional)**
   ```bash
   npm run dev
   ```

## 📖 Usage

### Tracking Time
- The extension automatically tracks time on each tab
- Click the extension icon to see time spent per page
- Use the toggle to pause/resume tracking

### Capturing Highlights
- Select any text on a webpage
- Right-click and choose "Save to Memory"
- View saved highlights in the extension popup

### Managing Data
- Search through saved entries
- Delete individual entries
- Clear all data with one click

## 🧪 Development

### Available Scripts

```bash
npm run dev       # Start Vite dev server
npm run build     # Build for production
npm run lint      # Run ESLint
npm run preview   # Preview production build
```

### Code Quality

This project uses ESLint to maintain code quality. Run linting before committing:

```bash
npm run lint
```

## 🔍 Key Learnings

- Managing state between popup, background, and content scripts
- Handling Chrome lifecycle events (tab creation, updates, closure)
- Preventing popup resize collapse issues
- Structuring scalable extension architecture
- Efficient data persistence with chrome.storage.local

## 🔐 Privacy & Security

- ✅ All data is stored **locally** on your machine
- ✅ No data is sent to external servers
- ✅ No telemetry or analytics
- ✅ No ads or tracking
- See [SECURITY.md](SECURITY.md) for more details

## 📋 Extension Permissions

This extension requests:
- **tabs** - To track active tab and browsing time
- **scripting** - To inject content scripts for text capture
- **storage** - To persist user data locally

No sensitive permissions beyond what's necessary for core functionality.

## 🚧 Future Improvements

- [ ] IndexedDB support for larger datasets
- [ ] Smarter highlight anchoring and context
- [ ] Unit and integration tests
- [ ] Export functionality (JSON/CSV)
- [ ] Dark mode support
- [ ] Keyboard shortcuts
- [ ] Cloud sync option (optional)
- [ ] Data visualization and statistics

## 🤝 Contributing

We welcome contributions! Please see [CONTRIBUTING.md](CONTRIBUTING.md) for guidelines on:
- Setting up development environment
- Making changes
- Submitting pull requests
- Reporting bugs and requesting features

## 🐛 Troubleshooting

### Extension not appearing
- Ensure you loaded it from the `dist/` folder, not `src/`
- Try refreshing the extension on `chrome://extensions`

### Changes not showing
- Run `npm run build` to rebuild
- Refresh the extension

### Storage not persisting
- Check that you have enough disk space
- Ensure the extension is not using incognito mode

### Context menu not appearing
- Restart Chrome
- Reload the extension from `chrome://extensions`

## 📚 Resources

- [Chrome Extension Documentation](https://developer.chrome.com/docs/extensions/)
- [Manifest V3 Migration Guide](https://developer.chrome.com/docs/extensions/mv3/migration/)
- [React Documentation](https://react.dev/)
- [TypeScript Documentation](https://www.typescriptlang.org/docs/)

## 📄 License

This project is licensed under the MIT License - see [LICENSE](LICENSE) for details.

## 👤 Author

**eswar06**

- GitHub: [@eswar06](https://github.com/eswar06)

## 📌 Acknowledgments

Built with:
- [Vite](https://vitejs.dev/) - Lightning fast build tool
- [React](https://react.dev/) - UI library
- [TypeScript](https://www.typescriptlang.org/) - Type safety
- [Chrome Extensions API](https://developer.chrome.com/docs/extensions/) - Extension platform

---

**If you find this project useful, consider giving it a ⭐**
