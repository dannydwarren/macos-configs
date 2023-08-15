# mac-configs

Steps to getting my MacOS ready for dev.

1. Install git and MacOS dev tools: `git`
    - ```code ~/.gitconfig```
    - Copy [danny.gitconfig](https://github.com/dannydwarren/machine-configs/blob/main/git/danny.gitconfig) into local `.gitconfig`
1. Create zsh profile: `touch ~/.zshrc`
1. Install brew: `/bin/bash -c "$(curl -fsSL https://raw.githubusercontent.com/Homebrew/install/HEAD/install.sh)"`
1. Install iterm2: `brew install --cask iterm2`
1. iTerm
1. Install Git Credential Manager (gcm)
    ```
    brew tap microsoft/git
    brew install --cask git-credential-manager-core
    ```
1. Install MS Edge: `brew install --cask microsoft-edge`
1. Install VS Code: `brew install --cask visual-studio-code`
1. Docker [for Mac](https://docs.docker.com/desktop/install/mac-install/)
   - [Download Docker Desktop Installer](https://desktop.docker.com/mac/main/amd64/Docker.dmg?utm_source=docker&utm_medium=webreferral&utm_campaign=docs-driven-download-mac-amd64&_gl=1*11tg1v6*_ga*NjU1NTc3OTAwLjE2ODkxMTA3Mzg.*_ga_XJWPQMJYHQ*MTY4OTExMDczOC4xLjEuMTY4OTExMDkxNS41MS4wLjA.)
   - ```
     cd ~/downloads
     sudo hdiutil attach Docker.dmg
     sudo /Volumes/Docker/Docker.app/Contents/MacOS/install
     sudo hdiutil detach /Volumes/Docker
     ```
    - Settings -> Advanced -> Run as User (and follow manual steps)
1. Install NVM: `brew install nvm`
    ```
    mkdir ~/.nvm
    nvm install 
    ```
    - Add nvm to `~/.zshrc`
       ```
       code ~/.zshrc
       # Write the following to the profile (uncommented)
       #export NVM_DIR="$HOME/.nvm"
       #    [ -s "$HOMEBREW_PREFIX/opt/nvm/nvm.sh" ] && \. "$HOMEBREW_PREFIX/opt/nvm/nvm.sh"
       #    [ -s "$HOMEBREW_PREFIX/opt/nvm/etc/bash_completion.d/nvm" ] && \. "$HOMEBREW_PREFIX/opt/nvm/etc/bash_completion.d/nvm"
       ```
1. Install dotnet
    - [.NET Core 3.1](https://download.visualstudio.microsoft.com/download/pr/c319dd8b-4ea5-473e-8609-c36f31c8186e/c9633afb3084888a8c62fa224512050b/dotnet-sdk-3.1.426-osx-x64.pkg)
1. Install node: `nvm install --lts`
1. Install yarn: `brew install yarn`
1. Install gulp: `npm install --global gulp-cli`
1. Install JetBrains Toolbox: [Download](https://www.jetbrains.com/toolbox-app/)
