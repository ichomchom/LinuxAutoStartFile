[3~# Script

This is the simple script to open the pdf, jpg file when users logon to computer.

## Getting Started

1. Put the script autostart.desktop in /etc/xdg/autostart.
2. Put the script autostart.sh in your desire folder.

### Changing PowerShell Script Location

Open batch.bat file

```
@echo off
mode con: cols=50 lines=10
Powershell.exe -executionpolicy remotesigned -File  \\samba\netlogon\logon.ps1
pause
```
Change ```\\samba\netlogon\``` as your desire location where you put the script logon.ps1.
