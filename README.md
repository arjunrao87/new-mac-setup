# install vscode cli 
- https://code.visualstudio.com/docs/setup/mac

# git clone ssh 
- ssh-keygen -t ed25519 -C "rao.arjun87@gmail.com"
- eval "$(ssh-agent -s)"
- touch ~/.ssh/config
- add to file 
```
Host github.com
  AddKeysToAgent yes
  UseKeychain yes
  IdentityFile ~/.ssh/id_ed25519
```
- pbcopy < ~/.ssh/id_ed25519.pub
- create key in github ssh (https://github.com/settings/ssh/new)

# terminal
- touch ~/.zshrc
- powerlevel10k
  - brew install powerlevel10k
  - echo "source $(brew --prefix)/share/powerlevel10k/powerlevel10k.zsh-theme" >>~/.zshrc
  - for more instructions --> https://github.com/romkatv/powerlevel10k?tab=readme-ov-file#homebrew
  - p10k configure

# tools 
- brew: /bin/bash -c "$(curl -fsSL https://raw.githubusercontent.com/Homebrew/install/HEAD/install.sh)"
  - (echo; echo 'eval "$(/opt/homebrew/bin/brew shellenv)"') >> /Users/arjunrao/.zprofile
  - eval "$(/opt/homebrew/bin/brew shellenv)"
- nvm: curl -o- https://raw.githubusercontent.com/nvm-sh/nvm/v0.39.7/install.sh | bash
- python: brew install python
  - add to ~/.zshrc :: export PATH="$PATH:/opt/homebrew/bin/"
  - which python3 
- node: brew install node 
  - npm install --global yarn

