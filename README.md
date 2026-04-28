# VibeForge v0.1.1 Beta Release
https://VibeForge.Online/

## Description
VibeForge is a high-performance, aesthetically pleasing multi-terminal project manager tailored for "AI Vibe Coding." It allows developers to manage multiple simultaneous AI sessions (like Claude CLI, Gemini CLI, or Codex) across different projects within a unified, grid-based workspace. VibeForge streamlines the workflow of iterating with AI by combining robust terminal emulation, a simplified file explorer, and a quick-access code editor into a single, cohesive interface.

## Currently Implemented Features

### 🚀 AI-Centric Workflow
- **Integrated AI Tools**: Pre-configured support for `Claude CLI`, `Codex CLI`, and `Gemini CLI`, with an optional "Bypass Mode" that allows launching Model with Permissions bypassed for power users (Requires accepting prompt acknowledging the risk of using the CLI bypass modes).
- **Auto-Bootstrapping**: New terminals automatically launch your preferred AI tool upon opening.
- **Global & Project Overrides**: Set a default AI tool globally or override it for specific projects.
- **Prompt Recommendations**: A built-in, quick-access guide with sample prompts for refactoring, feature implementation, bug hunting, and styling.

### 🖥️ Advanced Terminal Management
- **Multi-Terminal Grid**: Dynamic grid layout that automatically adjusts as you open or close project sessions.
- **True Terminal Emulation**: Powered by `xterm.js` and `node-pty` for a full-featured shell experience (CMD/PowerShell on Windows).
- **Persistent Sessions**: Terminals stay active and responsive even when switching between editor and explorer views.
- **Responsive Resizing**: Terminals automatically refit their dimensions when the window or layout changes.

### 📁 Project & File Management
- **Project Sidebar**: Easily browse, create, rename, duplicate, and delete projects within your designated root directory.
- **Integrated File Explorer**: A built-in explorer per terminal pane for navigating project structures without leaving the app.
- **Surgical Code Editor**: A lightweight, focused editor with built-in syntax highlighting (JS/TS/JSON/Python/C/C++/C#/HTML/CSS) for quick modifications and "vibe checks" during AI sessions.
- **Multi-Project Workspace**: Open and manage multiple different projects side-by-side in a single view.

### 🎨 Customization & Aesthetics
- **Theme Engine**: Deeply customizable UI with live-updating theme colors (Background, Sidebar, Accent).
- **Modern UI/UX**: Industrial-minimalist design with high-quality typography, smooth transitions, and a focus on "flow."
- **Collapsible Layouts**: Collapsible sidebars and explorers to maximize terminal real estate.
- **Frameless Window**: Custom title bar and window controls for a sleek, integrated desktop experience.

### ⚙️ Technical Foundation
- **Cross-Platform Base**: Built on Electron with Vite and React for high performance and low latency.
- **Local-First Architecture**: Uses `electron-store` for persistent settings and direct filesystem access for project management.
- **Resource Bundling**: Packaged with essential tools and guides for a zero-config start.

### VibeForge Release Notes - v0.1.1

## New Features
- **File Explorer Operations**: Full support for file and folder management directly from the sidebar.
  - **Create**: Add new files or folders to your project via header buttons or context menu.
  - **Rename**: Rename existing files and directories.
  - **Delete**: Move unwanted items to the system trash.
  - **Duplicate**: Quickly clone files or folders.
  - **Reveal**: Open the file's location in your OS file explorer.
- **Context Menu**: Added a modern right-click context menu for all entries and the explorer background.
  - Root/Empty Space: New File, New Folder, Reveal.
  - Folder actions: Expand/Collapse, New File, New Folder, Rename, Delete, Reveal.
  - File actions: Open, Rename, Delete, Duplicate, Reveal.
- **Terminal Reliability**: Enhanced terminal interaction with selection and clipboard support.
  - **Context Menu**: Right-click inside any terminal to Copy, Paste, or Clear the console.
  - **Shortcuts**: Support for `Ctrl+Shift+C` (Copy) and `Ctrl+Shift+V` (Paste) standard terminal hotkeys.

## UI/UX Improvements
- **Terminal Theming**: Added custom selection background matching the app's accent color for better visibility.
- **Explorer Header**: Added quick-access buttons for "New File" and "New Folder".
- **Empty Space Support**: Right-clicking in the empty area of the file tree now correctly opens a root-level context menu.
- **Enhanced Sidebar**: Improved visual feedback with hover states and better spacing for file tree entries.
- **Cross-Platform Consistency**: Improved path handling logic to ensure smooth operation across Windows, macOS, and Linux.
- **Dynamic Refresh**: The file tree now automatically updates its view after any file operation.

## Technical Changes
- **Native Clipboard Integration**: Switched to Electron's native `clipboard` module for improved reliability across all platforms.
- **IPC Expansion**: Added robust backend handlers in the Electron main process for secure file system manipulation and clipboard access.
- **Preload API Enhancement**: Exposed system-level path separators and new file utility methods to the renderer.
- **Global Styles**: Added centralized CSS for context menus and interactive tree elements.

## Bug Fixes
- **Fixed a bug with copy/pasting within the terminal sessions
- **Fixed a bug that would cause VibeForge To sometimes Remain Open in the background after being closed. Added code to ensure it always shuts down cleanly
