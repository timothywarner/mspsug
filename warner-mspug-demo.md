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

### **Debugging**

1. Open PowerShell samples folder
2. Switch to Debug view
3. Review launch.json config file
4.

### **Workspaces**

1. 







