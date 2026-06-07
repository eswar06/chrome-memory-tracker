# Changelog

All notable changes to this project will be documented in this file.

The format is based on [Keep a Changelog](https://keepachangelog.com/en/1.0.0/),
and this project adheres to [Semantic Versioning](https://semver.org/spec/v2.0.0.html).

## [0.1.0] - 2026-03-04

### Added
- Initial release of Chrome Memory Tracker
- Track time spent per page
- Save selected text via context menu
- Persistent local storage using chrome.storage.local
- Search functionality for saved entries
- Toggle tracking on/off
- Clear stored memory feature
- React-based popup UI
- TypeScript support for type safety
- Manifest V3 architecture
- Background service workers for efficient resource usage
- Content scripts for text selection capture
- ESLint configuration for code quality

### Technical Details
- Built with React 19 and TypeScript 5
- Vite as build tool with Rolldown
- Chrome Extensions API (Manifest V3)
- No external backend dependencies

---

## Unreleased

### Planned Features
- IndexedDB support for larger datasets
- Smarter highlight anchoring
- Unit tests for storage layer
- Export functionality (JSON/CSV)
- Dark mode support
- Keyboard shortcuts
- Cloud sync option
