# 🖥️ PowerShell Cheat Sheet

Quick reference for common PowerShell commands.

---

## 📂 File & Folder Management
| Command | Alias | Description |
|---------|-------|-------------|
| `Get-ChildItem` | `ls`, `dir` | List files and directories |
| `Set-Location` | `cd` | Change current directory |
| `Copy-Item file.txt C:\Path` | `cp` | Copy file or folder |
| `Move-Item file.txt C:\Path` | `mv` | Move file or folder |
| `Remove-Item file.txt` | `rm`, `del` | Delete file or folder |
| `New-Item -ItemType File -Name file.txt` | — | Create new file |
| `New-Item -ItemType Directory -Name Folder` | — | Create new folder |

---

## 🔍 System Information
| Command | Alias | Description |
|---------|-------|-------------|
| `Get-ComputerInfo` | — | Show system info (OS, CPU, RAM, BIOS) |
| `Get-Process` | `ps` | List running processes |
| `Get-Service` | — | List Windows services |
| `Get-EventLog -LogName System -Newest 10` | — | Show latest 10 system logs |
| `Get-WmiObject Win32_LogicalDisk` | — | Show disk info |

---

## ⚙️ Process & Task Management
| Command | Alias | Description |
|---------|-------|-------------|
| `Start-Process notepad` | — | Launch app/program |
| `Stop-Process -Name notepad` | — | Kill a process |
| `Get-Process \| Sort CPU -Descending \| Select -First 5` | — | Top 5 CPU-heavy processes |

---

## 👤 User & Security
| Command | Alias | Description |
|---------|-------|-------------|
| `Get-LocalUser` | — | List local users |
| `Get-LocalGroup` | — | List groups |
| `New-LocalUser "User" -Password (Read-Host -AsSecureString)` | — | Create new user |
| `Add-LocalGroupMember
