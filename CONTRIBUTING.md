# Contributing to Chrome Memory Tracker

Thank you for your interest in contributing! This document provides guidelines and instructions for contributing.

## Getting Started

1. **Fork the repository** on GitHub
2. **Clone your fork** locally:
   ```bash
   git clone https://github.com/YOUR_USERNAME/chrome-memory-tracker.git
   cd chrome-memory-tracker
   ```
3. **Create a branch** for your feature/fix:
   ```bash
   git checkout -b feature/your-feature-name
   ```

## Development Setup

1. Install dependencies:
   ```bash
   npm install
   ```
2. Start development server:
   ```bash
   npm run dev
   ```
3. Build for testing:
   ```bash
   npm run build
   ```
4. Run linter:
   ```bash
   npm run lint
   ```

## Making Changes

- Keep commits focused and atomic
- Use descriptive commit messages
- Follow the existing code style (TypeScript + ESLint)
- Test your changes thoroughly in Chrome before submitting

## Loading the Extension in Development

1. Run `npm run build`
2. Open Chrome and go to `chrome://extensions`
3. Enable "Developer mode"
4. Click "Load unpacked"
5. Select the `dist/` folder

## Submitting Changes

1. Push your branch to your fork
2. Open a Pull Request against the main repository
3. Provide a clear description of your changes
4. Link any related issues

## Code Style

- Use TypeScript for all code
- Follow ESLint configuration
- Use React hooks for component logic
- Keep components small and focused

## Bug Reports

When reporting bugs, please include:
- Browser version and OS
- Steps to reproduce
- Expected vs actual behavior
- Screenshots if applicable

## Feature Requests

Describe the feature, its use case, and how it would benefit users.

## Questions?

Feel free to open an issue for questions or discussions.

Thank you for contributing! 🎉
