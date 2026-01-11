# vscode

## settings.json

### Terminal 

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

### Behavior
```json
{
    // Defines how VS Code behaves when editing files.
    "files.autoSave": "onFocusChange",
}
```


### Appearance 

These settings disable visual guides and UI elements.

```json
{
// Disables indentation guide lines in the editor
"editor.guides.indentation": false,

// Hides the Command Center from the window title bar
"window.commandCenter": false,

// Sets the menu bar to a compact display mode
"window.menuBarVisibility": "compact",

// Disables the code minimap on the right side of the editor
"editor.minimap.enabled": false,

// Disables breadcrumb navigation (file path and symbols)
"breadcrumbs.enabled": false,

// Disables bracket pair colorization
"editor.bracketPairColorization.enabled": false,

// Disables visual guides for matching bracket pairs
"editor.guides.bracketPairs": false,

// Hides the close button on editor tabs
"workbench.editor.tabActionCloseVisibility": false
  
}
```


## Keyboard

```jsonc
// expands the current selection based on syntax/context
{ "key": "shift+alt+left", "command": "editor.action.smartSelect.expand", "when": "editorTextFocus" },
{ "key": "shift+alt+right", "command": "editor.action.smartSelect.expand", "when": "editorTextFocus" },

// navigate and edit text by word parts (ideal for camelCase and snake_case)
{ "key": "ctrl+backspace", "command": "deleteWordPartLeft", "when": "textInputFocus"},
{ "key": "ctrl+delete", "command": "deleteWordPartRight", "when": "textInputFocus" },
{ "key": "ctrl+right", "command": "cursorWordPartRight", "when": "textInputFocus"},
{ "key": "ctrl+left", "command": "cursorWordPartLeft", "when": "textInputFocus" },

// move the current line up or down
{ "key": "shift+alt+down", "command": "editor.action.moveLinesDownAction", "when": "textInputFocus" },
{ "key": "shift+alt+up", "command": "editor.action.moveLinesUpAction", "when": "textInputFocus" },

// copy the current line up or down
{ "key": "ctrl+shift+up", "command": "editor.action.copyLinesUpAction", "when": "textInputFocus" },
{ "key": "ctrl+shift+down", "command": "editor.action.copyLinesDownAction", "when": "textInputFocus" },

```




