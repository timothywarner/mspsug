# Transition Your PowerShell Work from ISE to Visual Studio Code

## Tim Warner ([@TechTrainerTim](https://twitter.com/techtrainertim); [TechTrainerTim.com](https://techtrainertim.com))

### **Why Not the ISE?**

* PowerShell ISE isn't compatible with PowerShell Core
* Microsoft's (most closely) [official statement](https://docs.microsoft.com/en-us/powershell/scripting/components/ise/introducing-the-windows-powershell-ise?view=powershell-6):

>"The ISE was first introduced with Windows PowerShell V2 and was redesigned with PowerShell V3. The ISE is supported in all supported versions of Windows PowerShell up to and including Windows PowerShell V5.1. The ISE, however, is in maintenance mode and no new features are likely to be added. Additionally, there is no support for the ISE with PowerShell v6 and beyond. Users wanting a graphical tool with which to manage PowerShell scripts, etc, should consider Visual Studio Code."

### **Installation**

1. Install [Git](https://git-scm.com/) first.
2. Install [PowerShell Core](https://docs.microsoft.com/en-us/powershell/scripting/install/installing-powershell-core-on-windows?view=powershell-6) while you're at it
3. Install [Visual Studio Code](https://code.visualstudio.com/) second.
4. Install the [PowerShell](https://marketplace.visualstudio.com/items?itemName=ms-vscode.PowerShell) extension third.
5. Install a couple more "core" extensions fourth:
    * [Settings Sync](https://marketplace.visualstudio.com/items?itemName=Shan.code-settings-sync)
    * [VSCode-Icons](https://marketplace.visualstudio.com/items?itemName=vscode-icons-team.vscode-icons)

### **Configuration**

1. Activate the ISE color theme
2. Activate the icons and test by opening the PowerShell samples folder
3. Go to Settings and adjust EDITOR and TERMINAL fonts
4. Show PowerShell options

Some useful settings:

```JSON
    "editor.mouseWheelZoom": true,
    "editor.minimap.enabled": false,
    "editor.renderWhitespace": "all",
    "editor.renderControlCharacters": true,
    "editor.wordWrap": "on",
    "editor.formatOnType": true,
    "editor.formatOnPaste": true,
```

### **Snippets**

1. Grab some [PowerShell snippets](https://rkeithhill.wordpress.com/2015/09/12/powershell-snippets-for-visual-studio-code/).
2. Open powershell.json
3. Paste in the snippets
4. To use, start a .ps1 file and do Command palette > Insert snippet

### **Key Bindings**

1. Open Gear > Keyboard Shortcuts
2. Set Run Selected
3. Set Run Active File
4. Set Show all Commands

Key binding assigned to a snippet:

```JSON
{
  "key": "cmd+k 1",
  "command": "editor.action.insertSnippet",
  "when": "editorTextFocus",
  "args": {
    "snippet": "console.log($1)$0"
  }
}
```

### PS Script Analyzer

1. Open a ps1 file
2. Command palette > PSScriptAnalyzer

### **Debugging**

1. Open PowerShell samples folder
2. Switch to Debug view
3. Review launch.json config file
4.

### **Workspaces**

1. Open folder
2. Add content
3. Save as workspace
4. Re-open workspace
5. Open workspace settings

Have the terminal open to that location:

```JSON
"terminal.integrated.cwd": "C:\Users\Tim\Desktop\Workspace"
```

### **Git**

1. Git init current workspace
2. You might want to consider using the Git Lens extension


### **Settings Sync**

1. Install [Settings Sync](https://marketplace.visualstudio.com/itemdetails?itemName=Shan.code-settings-sync) extension
2. Create personal access token at GitHub
3. Command palette > Sync > Upload


### **Final ISE "reaches"**

1. Consider [PowerShell Pro Tools](https://marketplace.visualstudio.com/itemdetails?itemName=ironmansoftware.powershellprotools) extension
2. I miss: [ISESteroids](http://www.powertheshell.com/isesteroids/)
3. I miss: [$psISE object](https://docs.microsoft.com/en-us/powershell/scripting/components/ise/object-model/the-ise-object-model-hierarchy?view=powershell-6)

