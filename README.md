# Kuality CLI — Homebrew Tap

Install the [Kuality](https://kuality.io) CLI to test any website for accessibility, performance, SEO, cross-browser compatibility, and 30+ QA dimensions from your terminal.

## Install

```bash
brew install --cask kuality-io/tap/kuality
```

## Usage

```bash
kuality scan <url> --type a11y --fail-on high
```

## Auth

Set your API key via environment variable or config file:

```bash
export KUALITY_API_KEY=ku_...
```

Or save it to `~/.kuality/config`.

## macOS Gatekeeper

On first run, macOS may block the binary with "kuality Not Opened" because it is not yet code-signed with an Apple Developer ID. Click **Done** (not "Move to Trash"), then remove the quarantine flag:

```bash
xattr -d com.apple.quarantine /opt/homebrew/Caskroom/kuality/0.1.0/kuality
```

## Links

- [kuality.io](https://kuality.io)
- [CLI documentation](https://kuality.io/docs/ci-api)
- [API reference](https://kuality.io/docs/sdk)
