# Lesson 0: Getting Started With Scientific Coding
---
## Objectives
- Learn How to Setup a GitHub Account
- Install Visual Studio Code
- Install Conda
- Install Docker
- Install Git
- Learn the Basics of Git
- Learn How to Configure a Conda Environment
---
### Setting Up a GitHub Account
[GitHub](https://github.com) is arguably the most popular remote repository hosting site for Git repositories. It is widely used by most individuals and organizations to collaborate on code, manage versions between multiple developers, and publish releases of software. Some alternatives include [GitLab](https://gitlab.com) and [Gitea](https://about.gitea.com/), but fundamentally they all serve the same purpose of providing a browser-based interface for git repositories.
1. Sign up for an account at this [link](https://github.com/signup) using a personal email.
 - A personal email is recommended, as you'll likely use GitHub far beyond your time at JHU.
---
### Installing Visual Studio Code
Visual Studio Code (VSCode for short) is a multi-language Integrated Development Environment (IDE) common across a large swathe of the software development world. It provides support for most programming languages via its extensions, and integration with useful tools such as linters, formatters, and debuggers. We'll expand on these additional useful tools later.
1. Download the Visual Studio Code installer at this [link](https://code.visualstudio.com/download?_exp_download=d53503e735).
2. Open Visual Studio Code and add the following extensions:
- Python
- Jupyter
---
### Installing Conda
Conda and its alternatives are tools for software version control common in the data science community. Reproducibility is the core principle of software version control. As behavior can change substantially between different versions of software, ensuring that subsequent researchers are using the same versions for an analysis helps guarantee that they can recreate any findings from it. A secondary benefit is reducing the chance of dependency conflicts, where multiple pieces of software depend on different versions of the same package. By isolating different versions of software into separate containers, different stages of analysis can coexist without issue.
1. Install [Anaconda](https://repo.anaconda.com/archive/Anaconda3-2026.07-1-Windows-x86_64.exe), [Miniconda](-https://anaconda.com/api/installers/Miniconda3-latest-Windows-x86_64.exe?attr=ZGxzb3VyY2U9d3d3LmFuYWNvbmRhLmNvbSZ0aW1lc3RhbXA9MjAyNi0xMC0xMlQxMiUzQTIwJTNBNDBaJnV0bV9jYW1wYWlnbj1OVUxMJnV0bV9jb250ZW50PU5VTEwmdXRtX21lZGl1bT1hbmFjb25kYSZ1dG1fc291cmNlPWRpcmVjdCZ1dG1fdGVybT1OVUxM&sig=384f7b9589063516884aa01e98ea7f6c4078590a644aa935b8b7afa9dd324821--), or [Mamba](https://github.com/conda-forge/miniforge/releases/download/26.7.2-0/Miniforge3-26.7.2-0-Windows-x86_64.exe).
 - Miniconda or Mamba are preferred over traditional Anaconda as they are smaller installations and tend to produce fewer bugs, and Mamba is substantially faster than the alternatives. Anaconda does provide a Graphical User Interface to ease its use however, and comes with a wide selection of pre-installed software.
2. During installation, make sure to make Conda (or Mamba) available on your PATH.
---
### Installing Docker
Docker is another tool for software version control, though it goes a step beyond Conda. While Conda is largely focused on the data science software ecosystem and only packages a select assortment of related tools, Docker can bundle an entire Linux operating system and any software which runs on it into a container. This is most useful when developing analyses for use on High-Performance Computing Clusters or powerful Linux workstations and servers, and it allows for development and testing in an environment that is identical between anyone who receives the container.
1. Open Powershell or Windows Command Prompt as an Administrator
2. Run `wsl --install` to install Windows Subsystem for Linux
3. Install Docker Desktop at this [link](https://desktop.docker.com/win/main/amd64/Docker%20Desktop%20Installer.exe).
4. In the installer, select Windows Subsystem for Linux as the backend.
---
### Installing Git
Git is the ubiquitous version control system for almost all software development and data analysis. It operates on a core principle of taking snapshots of points in time in a repository's history, called commits, and stacking them on top of one another to assemble a complete history of all changes across a repository's history. Git also provides the ability to branch off different versions of a repository, merge them back together, and much more, though we'll only scratch the surface of its capabilities today.
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

#### Setting up GitHub Authentication
1. Open a Git Bash terminal anywhere.
2. Run `winget install --id GitHub.cli --source winget`.
  - You may need to install winget from the App Installer, if it's not already available on your system.
  - This is installing the Github Credential Manager, allowing your local installation of Git to know what repositories you own on GitHub.
3. Run `gh auth login` and walk through the interactive process to authenticate with GitHub.
