# sMokeY

![Version](https://img.shields.io/badge/version-0.0.0-blue.svg)
![Electron](https://img.shields.io/badge/electron-latest-47848f.svg)
![CodeMirror](https://img.shields.io/badge/codemirror-6-orange.svg)
![Platform](https://img.shields.io/badge/platform-win%20%7C%20mac%20%7C%20linux-lightgrey.svg)
![License](https://img.shields.io/badge/license-MIT-green.svg)
![Mood](https://img.shields.io/badge/Mood-Sassy-purple.svg)


A simple, clean text editor for desktop.

## What it is

- Cross-platform text editor (Windows, Mac, Linux)
- Minimal interface, maximum focus
- Fast and lightweight
- Named after a sassy munchkin cat 🐱

## Tech Stack

- **Electron.js** - Desktop framework
- **CodeMirror 6** - Text editing engine
- **Anonymous Pro** - Monospace font
- **Node.js** - Build system

## Features

- Auto-save
- Find/replace
- Line numbers (optional)
- Word wrap
- Dark/light themes
- Sliding toolbar (appears on hover)
- Real-time file watching

## Quick Start

```bash
git clone https://github.com/spenceriam/sMokeY
cd smokey
npm install
npm start
```

## Build

```bash
npm run build
```

## Shortcuts

- `Ctrl/Cmd + N` - New
- `Ctrl/Cmd + O` - Open  
- `Ctrl/Cmd + S` - Save
- `Ctrl/Cmd + F` - Find
- `Ctrl/Cmd + Z` - Undo

## Structure

```
smokey/
├── src/
│   ├── main/      # Electron main process
│   └── renderer/  # UI and editor
├── assets/        # Fonts and icons
└── builds/        # Output builds
```

---

Simple. Clean. Just like sMokeY likes it.
