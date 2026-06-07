# Security Policy

## Reporting Security Vulnerabilities

If you discover a security vulnerability in Chrome Memory Tracker, please email the maintainer privately instead of using the public issue tracker.

**Do not open public issues for security vulnerabilities.**

Please provide:
- Description of the vulnerability
- Steps to reproduce
- Potential impact
- Any suggested fixes

## Security Considerations

### Data Privacy
- All data is stored locally using `chrome.storage.local`
- No data is sent to external servers
- No telemetry or analytics

### Permissions
This extension requests:
- `tabs` - To track active tab and time spent
- `scripting` - To inject content scripts for text selection capture
- `storage` - To persist user data locally

### Content Security Policy
The extension follows Chrome's Content Security Policy guidelines:
- No inline scripts
- No unsafe-eval
- React compiled without eval

## Best Practices

When using this extension:
- Install from official sources only
- Keep your Chrome browser updated
- Review extension permissions before installation
- Report suspicious behavior

## Extension Manifest

The extension uses **Manifest V3**, which provides enhanced security over previous versions:
- Background service workers instead of persistent background pages
- Restricted eval-like functions
- Secure context requirements

---

For any security concerns, please contact the maintainer privately.
