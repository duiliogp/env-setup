# vscode

## settings.json

### Behavior

Switch the integrated terminal to Git Bash.

```json
{
  "terminal.integrated.defaultProfile.windows": "Git Bash",
  "terminal.integrated.profiles.windows": {
    "Git Bash": {
      "path": "C:\\Program Files\\Git\\bin\\bash.exe"
    }
  }
}
```

Changes the cursor style and blinking behavior of the integrated terminal.
```jsonc
{
    "terminal.integrated.cursorStyle": "line",
    "terminal.integrated.cursorBlinking": true,
}
```

Defines how VS Code behaves when editing files.
```json
{
    "files.autoSave": "onFocusChange",
}
```


### Appearance 

These settings turn off certain visual guides and UI elements:

```json
{
  "editor.guides.indentation": false,
  "window.commandCenter": false,
  "window.menuBarVisibility": "compact",
  "editor.minimap.enabled": false,
  "breadcrumbs.enabled": false,
  "editor.bracketPairColorization.enabled": false,
  "editor.guides.bracketPairs": false,
  "workbench.editor.tabActionCloseVisibility": false, // Hides the close (X) button on tabs;close tabs with middle-click (scroll button)
}
```


