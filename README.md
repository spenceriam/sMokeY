# sMokeY

![Version](https://img.shields.io/badge/version-0.0.0-blue.svg)
![Electron](https://img.shields.io/badge/electron-latest-47848f.svg)
![CodeMirror](https://img.shields.io/badge/codemirror-6-orange.svg)
![Platform](https://img.shields.io/badge/platform-win%20%7C%20mac%20%7C%20linux-lightgrey.svg)
![License](https://img.shields.io/badge/license-MIT-green.svg)
![Mood](https://img.shields.io/badge/Mood-Sassy-purple.svg)

<p align="center">
<img src="/logo.jpg" width=300>
</p>
<p align="center">
A simple, clean text editor for desktop.
</p>

## What it is

- Cross-platform text editor (Windows, Mac, Linux)
- Minimal interface, maximum focus
- Fast and lightweight
- Named after a sassy munchkin cat 🐱

## Tech Stack

- **Electron.js** - Desktop framework
- **CodeMirror 6** - Text editing engine
- **Node.js** - Build system

## Prompt used
Initial setup:
1. Clone down this Github repo into a location on your machine
2. With your choice of editor/IDE, open project
3. Kick off the project by scaffolding the structure:\
_Create a basic Electron application called 'sMokeY' with CodeMirror 6 text editor. Set up the project with proper folder structure, package.json with cross-platform build scripts, and a minimal working text editor that can open, edit, and save files. Include basic Electron security best practices and make sure it runs with 'npm start'. Keep the UI clean and minimal - just the editor for now._
5. Start the todo.md and then vibe on:\
_Based on this sMokeY text editor project, create a detailed todo.md file that breaks down all the remaining features into small, actionable chunks. Organize by priority and dependencies. Each task should be specific enough for AI to implement (like 'Add auto-save with 3-second interval' rather than 'Add auto-save'). Reference the PRD requirements for the complete feature list._

## Suggestions:
Create a rule file or memory:
- Manage the project using the todo and create a changelog from [(www.keepachangelog.com](https://keepachangelog.com/en/1.1.0/)

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
