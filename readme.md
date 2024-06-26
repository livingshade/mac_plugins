# Plugins & Command to make mac easy to use

Here are some Mac plugins or commands I've collected to get used to when switching from Windows

## Necessary Software

1. [Homebrew](https://brew.sh/)
2. [iRightMouse](https://www.irightmouse.com/)
3. [Snipaste](https://zh.snipaste.com/)
4. [Linearmouse](https://linearmouse.org/)
5. [Alfred](https://www.alfredapp.com/)
6. [Stretchly](https://hovancik.net/stretchly/)
7. [Karabiner](https://karabiner-elements.pqrs.org/)

   See myshortcut.json for my configuration
8. [iTerm2](https://iterm2.com/)
9. [AltTab](https://alt-tab-macos.netlify.app/)
10. [Rectangle](https://rectangleapp.com/)
11. [Command X](https://sindresorhus.com/command-x)
12. [CommandQ](https://commandqapp.com/)
## Settings

### Show breadcrumbs navigator in finder

Finder > View > Show Path Bar

### Auto switch input method

System Preferences > Keyboard > Input Sources > Automiacally switch to a document's input source

### Use ziranma(自然码双拼)

defaults write com.apple.inputmethod.CoreChineseEngineFramework shuangpinLayout 5

### Use xiaohe(小鹤双拼)

This is automatically supported in macOS `input source` settings

### zsh config

see .zshrc

### Globally ignore .DS_Store

```bash
echo ".DS_Store" >> ~/.gitignore_global
```

add following to ~/.gitconfig

```bash
[core]
   excludesfile = "~/.gitignore_global"
```

### Remove multiple version of edge at System Preferences > General > Default Web Browser

delete old edge folders in `~/Library/Microsoft/EdgeUpdater`
and `~/Library/Application Support/Microsoft/EdgeUpdater/apps/msedge-stable/`

### Find the bundle ID of an app

```bash
osascript -e 'id of app "App Name"'
```


### How to solve “Clash for Windows” is damaged and can’t be opened. You should move it to the Trash.

```bash
sudo xattr -r -d com.apple.quarantine /Applications/Clash\ for\ Windows.app
```

### Sort files and folders like Windows in Finder

Finder > Settings > Advanced > Keep folders on top when sorting by name

### Open in VSCode from Finder

Use mac automation, check this [link](https://www.youtube.com/watch?v=dcjevVMhpoM&ab_channel=MerillFernando)
