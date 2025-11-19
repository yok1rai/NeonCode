# 🚀 CyberPunk Themed VS Code Setup

A futuristic, neon-drenched Visual Studio Code theme and configuration that transforms your editor into a cyberpunk-inspired development environment.

## 📋 Prerequisites & Dependencies

### Required Extensions:
1. **Theme**: [Tokyo Night Storm](https://marketplace.visualstudio.com/items?itemName=enkia.tokyo-night)
   ```bash
   code --install-extension enkia.tokyo-night
   ```

2. **Icons**: [vscode-icons](https://marketplace.visualstudio.com/items?itemName=vscode-icons-team.vscode-icons)
   ```bash
   code --install-extension vscode-icons-team.vscode-icons
   ```

3. **Recommended Fonts** (install one or more):
   - [JetBrains Mono](https://www.jetbrains.com/lp/mono/)
   - [Fira Code](https://github.com/tonsky/FiraCode)

### Optional Extensions:
- **Live Server** (for web development)
- **Code Runner** (for executing code snippets)

## 🎯 What This Setup Provides

### 🎨 Visual Features:
- **Dark cyberpunk background** (#0d0f1a - deep space blue)
- **Neon accent colors** (magenta, cyan, electric green, yellow)
- **Colorized bracket pairs** with rainbow highlighting
- **Custom syntax highlighting** for different code elements
- **Minimal, distraction-free interface**

### ⚡ Performance & Behavior:
- **Auto-save** and **auto-format** on save
- **Smart suggestions** without AI bloat
- **Smooth scrolling** and animations
- **Efficient terminal** with persistent sessions
- **Quick file navigation** with breadcrumbs

## 🛠️ How to Use This Setup

### Method 1: Manual Setup
1. Copy the entire `settings.json` content
2. Open VS Code Settings (Ctrl+, / Cmd+,)
3. Click the "Open Settings (JSON)" icon in the top-right
4. Replace contents with the provided JSON
5. Save and restart VS Code

### Method 2: Profile Import
1. Open Command Palette (Ctrl+Shift+P / Cmd+Shift+P)
2. Search for "Preferences: Open Settings (JSON)"
3. Replace content and save

## ⚙️ Key Settings Explained

### Editor Configuration:
- **Font**: JetBrains Mono with ligatures
- **Font Size**: 15px with 1.6 line height
- **Tab Size**: 4 spaces with auto-detection
- **Word Wrap**: Enabled for long lines
- **Minimap**: Enabled with block rendering

### Workflow Enhancements:
- **Auto-save**: Saves after short delay
- **Format on Save/Paste**: Automatic code formatting
- **Code Actions**: Organizes imports and fixes issues on save
- **Sticky Scroll**: Keeps context visible while scrolling

### Terminal Setup:
- **Font**: JetBrains Mono, 14px
- **Block cursor** with blinking
- **Left-side tabs** for better navigation
- **5000 lines** of scrollback history

## 🎨 Customization Guide

### Changing Colors:
Modify the `workbench.colorCustomizations` section:
```json
"workbench.colorCustomizations": {
    "editor.background": "#YOUR_COLOR",
    "editor.foreground": "#YOUR_COLOR",
    // ... other color overrides
}
```

### Adjusting Syntax Colors:
Edit the `editor.tokenColorCustomizations` section:
```json
"editor.tokenColorCustomizations": {
    "textMateRules": [
        {
            "scope": ["keyword"],
            "settings": {
                "foreground": "#YOUR_COLOR",
                "fontStyle": "bold"
            }
        }
    ]
}
```

### Font Customization:
Change the font family in these locations:
- `editor.fontFamily`
- `terminal.integrated.fontFamily`

## 🌍 Making It Global

### Option 1: Settings Sync
1. Enable VS Code Settings Sync
2. Sync across all your machines automatically

### Option 2: Manual Global Application
1. Place `settings.json` in:
   - **Windows**: `%APPDATA%\Code\User\settings.json`
   - **macOS**: `~/Library/Application Support/Code/User/settings.json`
   - **Linux**: `~/.config/Code/User/settings.json`

### Option 3: Create a Settings Profile
1. Open Command Palette
2. Search for "Preferences: Create Profile"
3. Import settings and apply to new workspaces

## 🔧 Troubleshooting

### Common Issues:

1. **Theme not appearing?**
   - Ensure Tokyo Night Storm extension is installed
   - Restart VS Code after installation

2. **Fonts not working?**
   - Install JetBrains Mono or Fira Code on your system
   - Check font name spelling in settings

3. **Colors look wrong?**
   - Disable other theme extensions that might conflict
   - Check if color customization syntax is correct

4. **Performance issues?**
   - Disable minimap: `"editor.minimap.enabled": false`
   - Reduce smooth scrolling: `"editor.smoothScrolling": false`

## 📁 File Structure
```
.vscode/
└── settings.json          # Main configuration file
README.md                  # This documentation
```

## 🎮 Quick Tips
- Use `Ctrl+Shift+P` → "Developer: Reload Window" to apply changes
- Toggle terminal with `` Ctrl+` ``
- Use breadcrumbs for quick file navigation
- Customize further based on your specific language needs

## 🔗 Resources
- [GitHub Repository](https://github.com/yok1rai/Cyberpunk_themed_VSCode)
- [VS Code Settings Documentation](https://code.visualstudio.com/docs/getstarted/settings)
- [Tokyo Night Theme](https://github.com/enkia/tokyo-night-vscode-theme)

---

**Enjoy your cyberpunk coding experience!** 🦾⚡
