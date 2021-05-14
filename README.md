# Managing Files

[![Contributor Covenant](https://img.shields.io/badge/Contributor%20Covenant-v1.4%20adopted-ff69b4.svg)](code-of-conduct.md)
[![License: MIT](https://img.shields.io/badge/License-MIT-green.svg)](https://opensource.org/licenses/MIT)

> Basic file management skills

## Organizing Files

File systems arrange files in a tree structure, with a single root directory.
A computer may be partitioned into multiple drives, if so, each drive will have its own root. 
Typically, there is a designated place to store user-created files. 
In Mac and Linux machines, it's the 'home' folder.
In Windows machines, it's the 'Documents' folder.
Under here, the user may create folders for a degree program, and under that folder, users may create sub-folders, one for each of your courses.

---

## Working with Files on Windows

On Windows, we can use either:

- File Explorer: a graphical interface (where we can use the mouse).
- PowerShell: a command line interface (where we can type commands).

### File Explorer (Graphical Interface)

The Windows File Explorer is a graphical way of browsing files.
Use this along with the PowerShell command line interface (CLI).
Folders and files can be added, edited, and deleted in File Explorer as well.

### PowerShell (Command Interface)

 We can use PowerShell to create, delete, and rename folders, sub-folders, and files. It's a powerful tool for organizing your files.
PowerShell offers aliases (shortened names) for common commands.
The full name is provided for additional reference [1].

- mkdir - create new folder/directory [Create-Item]
- cd - change directory [Set-Location]
- cd .. - cd up to immediate parent (cd ..\.. to go up 2 levels)
- rm - remove [Remove-Item]
- rni - rename item [Rename-Item]
- ni - new item [New-Item] - even shorter than Bash 'touch' command!
- ls - list contents [Get-ChildItem]
- clear - clear the history of commands [Clear-Host]

### Open PowerShell in User Folder

Use File Explorer to open your user folder (e.g. C:\Users\acctname).
Right-click on the folder itself (showing your account name) or in the white space off to the right.

Select "Open PowerShell window here as administrator" from the context menu.
If this is not yet available, see [Windows Setup for Developers](https://github.com/denisecase/windows-setup) to add this command to your context menu.

---

## Working with Folders

"Folders" and "directories" are the same and the terms can be used interchangeably.
When using the commands, it can be helpful to think in terms of "directories".
Try the following tasks - the commands are listed below.

1. In your default user folder, create a new folder/directory named "projects".
2. Try to create it again (the command should fail).
3. Change into your new directory.
4. Make several subdirectories.
5. Move into the first subdirectory.
6. Create an empty file (new item).
7. Create another child directory.
8. Rename it.
9. Delete it.
10. Back up to your projects directory.
11. Back up to your user directory.

```PowerShell
mkdir projects
mkdir projects
cd projects
mkdir proj1
mkdir proj2
mkdir proj3
cd proj1
ni README.md
mkdir startup
rni startup startingup
rm startingup
cd ..
cd ..
```

---

## Terms

- Drive
- File
- File Explorer - Windows program for browsing folders and files
- Folder / directory - a place to store files on your computerf
- PowerShell - powerful command line interface for Windows
- Tree data structure (every node has exactly one parent, except the root node with no parent)
- Windows 10 - popular operating system

## Next Steps

Now it's time to install some basic tools and software.

- Follow [Basic Tools](https://github.com/denisecase/basic-tools-for-webdev) to get some of the most common tools for professional software development.

## See Also

- [PowerShell Documentation](https://docs.microsoft.com/en-us/powershell/scripting/powershell-scripting?view=powershell-6)
