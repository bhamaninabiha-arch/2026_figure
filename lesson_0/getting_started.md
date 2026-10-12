# Getting Started
---
## Objectives
- Learn How to Setup a Github Account
- Install Visual Studio Code
- Install Conda
- Install Docker
- Install Git
- Learn the Basics of Git
- Learn How to Configure a Conda Environment
---
# Setting Up a Github Account
1. Sign up for an account at this [link](https://github.com/signup) using a personal email.
 - A personal email is recommended, as you'll likely use Github far beyond your time at JHU.
---
# Installing Visual Studio Code
1. Download the Visual Studio Code installer at this [link](https://code.visualstudio.com/download?_exp_download=d53503e735).
2. Open Visual Studio Code and add the following extensions:
- Python
- Jupyter
---
# Installing Conda
1. Install [Anaconda](https://repo.anaconda.com/archive/Anaconda3-2026.07-1-Windows-x86_64.exe), [Miniconda](-https://anaconda.com/api/installers/Miniconda3-latest-Windows-x86_64.exe?attr=ZGxzb3VyY2U9d3d3LmFuYWNvbmRhLmNvbSZ0aW1lc3RhbXA9MjAyNi0xMC0xMlQxMiUzQTIwJTNBNDBaJnV0bV9jYW1wYWlnbj1OVUxMJnV0bV9jb250ZW50PU5VTEwmdXRtX21lZGl1bT1hbmFjb25kYSZ1dG1fc291cmNlPWRpcmVjdCZ1dG1fdGVybT1OVUxM&sig=384f7b9589063516884aa01e98ea7f6c4078590a644aa935b8b7afa9dd324821--), or [Mamba](https://github.com/conda-forge/miniforge/releases/download/26.7.2-0/Miniforge3-26.7.2-0-Windows-x86_64.exe).
 - Miniconda or Mamba are preferred over traditional Anaconda as they are smaller installations and tend to produce fewer bugs, and Mamba is substantially faster than the alternatives.
---
# Installing Docker
1. Open Powershell or Windows Command Prompt as an Administrator
2. Run `wsl --install` to install Windows Subsystem for Linux
3. Install Docker Desktop at this [link](https://desktop.docker.com/win/main/amd64/Docker%20Desktop%20Installer.exe).
4. In the installer, select Windows Subsystem for Linux as the backend.
---
# Installing Git
1. Install Git for Windows at this [link](https://github.com/git-for-windows/git/releases/download/v2.56.0.windows.2/Git-2.56.0.2-64-bit.exe).
2. In the installer, ensure the following configuration options are enabled:
 - Git Bash
 - Git GUI
 - Git LFS
 - Windows Explorer Integration (Git Bash Here + Git GUI Here)
 - Associate .git* configuration files with the default text editor
 - Associate .sh files to be run with Bash
3. Select Visual Studio Code as Git's default editor
4. Override the default branch name for new repositories to `main`
5. Select to use Git from the command line and also from 3rd-Party Software
6. Select to use the bundled OpenSSH
7. Select to use the OpenSSL Library
8. Select to checkout Windows-style, commit Unix-style line endings
9. Select the `Default` git pull behavior

