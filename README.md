# Win11-Tweak-Guide
My personal tweak guide for everytime I fresh install Windows OS

## [Chris Titus Tech's Window Utility](https://github.com/ChrisTitusTech/winutil)

An AIO utility for your system. It includes installation of apps, enabling and disabling of features and configurations. 

### Almost everything in **Essential Tweaks** with exceptions of:
- Disable Hibernation
- Enable End Task with Right Click
- Replace Powershell 5 with Powershell 7 (Optional)

### Nothing much to configure in **Advanced Tweaks** except for:
- Adobe Network Block
- Adobe Debloat
- Disable Intel MM
- Set Display to Performance
- Set Time to UTC for Dual Boot
- Remove OneDrive

> [!NOTE]
> The Remove MS Edge option did not work

### For **OO Shutup10**:

Go to Local Machine to affect all users and enable the following:

- Everything in **Privacy**, **Activity History and Clipboard**, **Microsoft Edge (Legacy)**, **Cortana**, **Windows Explorer**, **Windows Copilot**, **Location Services**, **User Behavior**, and **Taskbar**
- Everything in **Security** besides `DRM`
- Everything in **Microsoft Defender and SpyNet** besides `reporting of malware and infection information`
- Everything in **Miscellaneous** besides `Key Management Service Online Activation`
- Set everything to default in **App Privacy** besides `user account information`, `diagnostics information`, `phone calls`, `call history`, `radios`, and `contacts`
- Set everything to default in **Windows Update**

## [Win11Debloat](https://github.com/Raphire/Win11Debloat)

Great for uninstalling pre-install applications.

### Usage

In powershell, run the command: 
```ps1
 & ([scriptblock]::Create((irm "https://win11debloat.raphi.re/"))) 
```

and set the mode to `Option 3` to proceed

## [EdgeRemover](https://github.com/he3als/EdgeRemover)

A script for removing Edge and WebView

### Usage

In powershell, run the command:
```ps1
iex(irm https://cdn.jsdelivr.net/gh/he3als/EdgeRemover@main/get.ps1)
```

and type `1` to enable the removal of edge user data and type `2` to proceed

## [Set Drag and Drop Action to Move](https://www.elevenforum.com/t/change-default-drag-and-drop-action-in-windows-11.2924/#3)

Changes the default mode of drag and drop action for folders and files to move instead of copying

### Usage

Download the `Drag&DropDefaultSetToMove` REG file and open it and restart `Explorer`

## [Remove Copilot](https://www.elevenforum.com/t/completely-disable-and-remove-copilot-in-windows-11.23264/)

Changes the default mode of drag and drop action for folders and files to move instead of copying

### Usage

Download the `RemoveCopilotFromAllUsers` REG file and open it and restart `Explorer`

To undo it, do the same for `UndoCopilotRemove` REG file

## [Remove Dev Home (Preview)](https://www.elevenforum.com/t/uninstall-or-reinstall-dev-home-app-in-windows-11-and-windows-10.18397/)

Removes the Dev Home (Preview) app

### Usage

In Powershell, run the command:
```ps1
Get-AppxPackage *Windows.DevHome* | Remove-AppxPackage
```

