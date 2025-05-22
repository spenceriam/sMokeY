# sMokeY - Product Requirements Document
**Product Name**: sMokeY 

## Product Overview

sMokeY is a lightweight, cross-platform desktop text editor designed for simplicity and focus. Named after a sassy munchkin cat, sMokeY embodies the same minimalist philosophy - clean, efficient, and distraction-free.

### Mission
Create a text editor that gets out of your way, letting you focus on writing without unnecessary complexity or visual clutter.

### Design Philosophy
- **Simplicity over features** - Essential functionality only
- **Performance over polish** - Fast and lightweight
- **Focus over distraction** - Zen-inspired minimal interface
- **Reliability over innovation** - Stable, predictable behavior

## Technical Specifications

### Core Framework
- **Platform**: Electron.js (latest stable)
- **Text Engine**: CodeMirror 6
- **Build System**: Node.js with npm scripts
- **Target Platforms**: Windows 10+, macOS Big Sur+, Linux (Ubuntu 20.04+)

### Performance Requirements
- **Startup Time**: < 3 seconds on average hardware
- **Memory Usage**: Lightweight for older devices
- **File Size Limit**: 800MB with user warning
- **Responsiveness**: UI interactions < 100ms response time

### Security & Compliance
- Modern Electron security practices
- Context isolation enabled
- Node.js integration disabled in renderer
- Secure IPC for file operations

## Core Features

### File Management
- **New File**: Create untitled documents
- **Open File**: Browse and select text files
- **Save/Save As**: Standard save operations with shortcuts
- **Auto-save**: Automatic saving with 3-second interval
- **Recent Files**: Track and display last 5 opened files
- **File Watching**: Real-time detection of external file changes
- **Conflict Resolution**: Handle simultaneous edit conflicts

### Text Editing
- **Basic Operations**: Cut, copy, paste, select all
- **Undo/Redo**: Full history with platform-specific shortcuts
- **Find/Replace**: Search within active document (Ctrl/Cmd+F)
- **Line Numbers**: Optional display (disabled by default)
- **Word Wrap**: Automatic text wrapping (enabled by default)
- **Text Selection**: Standard selection behaviors

### User Interface
- **Minimal Design**: Clean, distraction-free layout
- **Sliding Toolbar**: Hidden by default, appears on hover
- **Icon-Based Controls**: Intuitive toolbar with hover tooltips
- **Theme Support**: Dark and light mode toggle
- **Font System**: Anonymous Pro primary, system font fallbacks
- **Window Management**: Single window or optional tabbed interface

### Cross-Platform Features
- **Keyboard Shortcuts**: Platform-appropriate key combinations
- **File Paths**: Auto-detect Windows vs Unix path formats
- **Native Integration**: System dialogs and file associations (user choice)
- **Font Handling**: Embedded Anonymous Pro with graceful fallbacks

## Technical Architecture

### Process Structure
- **Main Process**: Application lifecycle, file I/O, window management
- **Renderer Process**: UI rendering, text editing, user interactions
- **IPC Communication**: Secure message passing between processes

### Data Storage
- **User Preferences**: Electron's built-in configuration storage
- **Session Data**: Window position, recent files, editor state
- **File Encoding**: UTF-8 default with encoding detection
- **Line Endings**: Auto-detect and preserve CRLF vs LF

### Key Components
- **File Manager**: Handles all file operations and watching
- **Editor Core**: CodeMirror 6 integration and configuration  
- **UI Controller**: Manages sliding toolbar and theme switching
- **Settings Manager**: User preference storage and retrieval
- **Conflict Resolver**: Handles external file change conflicts

## User Experience Requirements

### Interaction Design
- **Hover Interactions**: Toolbar appears on mouse hover at top/left edges
- **Smooth Animations**: 200ms transitions for UI state changes
- **Visual Feedback**: Clear indicators for auto-save, conflicts, etc.
- **Error Handling**: Graceful error messages with recovery options

### Accessibility
- **Keyboard Navigation**: Full keyboard accessibility
- **Screen Reader Support**: Proper ARIA labels and structure
- **High Contrast**: Theme support for accessibility needs
- **Font Scaling**: Respect system font size preferences

### Customization
- **Theme Selection**: Dark/light mode toggle
- **Font Choice**: Anonymous Pro default, system font selector
- **Editor Preferences**: Line numbers, word wrap, auto-save interval
- **Window Behavior**: Single vs multi-window preference

## Platform-Specific Considerations

### Windows
- **File Associations**: Optional .txt default handler
- **Keyboard Shortcuts**: Ctrl-based shortcuts
- **Window Controls**: Standard Windows window decorations
- **Installation**: MSI or NSIS installer

### macOS  
- **Keyboard Shortcuts**: Cmd-based shortcuts
- **Window Management**: Standard macOS window behavior
- **Menu Integration**: Native application menu
- **Installation**: DMG with drag-to-Applications

### Linux
- **Package Formats**: AppImage, .deb, .rpm support
- **Desktop Integration**: .desktop file for app launchers
- **Keyboard Shortcuts**: Ctrl-based shortcuts
- **Theme Integration**: Respect system theme preferences

## Update & Distribution

### Version Management
- **Semantic Versioning**: Major.Minor.Patch format
- **Update Checking**: Compare against GitHub releases
- **Manual Updates**: Direct users to download page
- **Change Notifications**: In-app update availability alerts

### Distribution Channels
- **GitHub Releases**: Primary distribution method
- **Direct Download**: From project website
- **Package Managers**: Future consideration for Linux
- **Platform Stores**: Future consideration for broader reach

## Quality Assurance

### Testing Requirements
- **Cross-Platform Testing**: Verify functionality on all target platforms
- **File Format Testing**: Various text encodings and line endings
- **Performance Testing**: Large file handling and memory usage
- **User Experience Testing**: UI responsiveness and accessibility

### Success Metrics
- **Performance**: Sub-3-second startup time maintained
- **Reliability**: Zero data loss in file operations
- **Usability**: Intuitive interface requiring no documentation
- **Compatibility**: Works consistently across all target platforms

## Future Considerations

Documented in `FUTURE.md` - features to consider post-MVP:
- Session restoration
- Syntax highlighting
- Multiple tabs/split view
- Plugin system
- Advanced find features
- Export capabilities

## Development Guidelines

### Code Quality
- Modern JavaScript (ES6+) 
- Clear, documented code structure
- Consistent naming conventions
- Error handling for all operations

### AI Development Approach
- Break features into discrete, implementable chunks
- Document AI prompting strategies and results
- Maintain human oversight for critical functionality
- Test thoroughly on all platforms

---

*Simple. Clean. Just like sMokeY likes it.*
