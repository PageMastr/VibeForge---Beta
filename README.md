# VibeForge v0.1.0 Beta Release
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
