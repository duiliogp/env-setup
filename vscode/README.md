# vscode

## settings.json

### Terminal 
```jsonc
{
    // Switch the integrated terminal to Git Bash.
    "terminal.integrated.defaultProfile.windows": "Git Bash",
    "terminal.integrated.profiles.windows": {
        "Git Bash": {
        "path": "C:\\Program Files\\Git\\bin\\bash.exe"
        }
    },

    // Changes the cursor style and blinking behavior of the integrated terminal.
    "terminal.integrated.cursorStyle": "line",
    "terminal.integrated.cursorBlinking": true,
    
    // Integrated terminal: disables sticky command headers while scrolling
    "terminal.integrated.stickyScroll.enabled": false,
}

### Behavior
```jsonc
{
    "files.autoSave": "onFocusChange",
    "chat.agent.enabled": false,
    "editor.hover.delay": 2000,
}
```


### Appearance 

These settings disable visual guides and UI elements.

```jsonc
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
"workbench.editor.tabActionCloseVisibility": false,

// Editor: disables sticky headers (keeps methods, classes, etc. from sticking at the top)
"editor.stickyScroll.enabled": false,

// Explorer / Tree views: disables sticky folders and items while scrolling
"workbench.tree.enableStickyScroll": false,

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


// show or hide core VS Code interface elements
{ "key": "ctrl+m", "command": "workbench.action.toggleStatusbarVisibility" },
{ "key": "ctrl+shift+L", "command": "workbench.action.toggleActivityBarVisibility" },

// insert a new line below the current line without moving existing text
{ "key": "shift+enter", "command": "editor.action.insertLineAfter", "when": "editorTextFocus && !editorReadonly" },
 { "key": "shift+enter", "command": "-editor.action.goToDeclaration", "when": "editorHasDefinitionProvider && editorTextFocus && !isInEmbeddedEditor" },

```




