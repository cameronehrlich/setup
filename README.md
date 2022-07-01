# Install Chrome

# Install Visual Studio Code
# - https://code.visualstudio.com/download
# - Install GitHub Copilot
# - Install "Shell Command install 'code' command in PATH"

# Install Homebrew
/bin/bash -c "$(curl -fsSL https://raw.githubusercontent.com/Homebrew/install/HEAD/install.sh)"

# Install ZSH
brew install zsh

# Install Oh-My-ZSH
sh -c "$(curl -fsSL https://raw.githubusercontent.com/robbyrussell/oh-my-zsh/master/tools/install.sh)"

brew install zsh-completions

# Install GitHub CLI
brew install gh
# gh auth login
# gh ssh-key add

# Install RVM
brew install gpg
gpg --keyserver hkp://pool.sks-keyservers.net --recv-keys 409B6B1796C275462A1703113804BB82D39DC0E3 7D2BAF1CF37B13E2069D6956105BD0E739499BDB
\curl -sSL https://get.rvm.io | bash --ruby
# Or if that doesn't work...
curl -sSL https://rvm.io/mpapis.asc | gpg --import - 
\curl -sSL https://get.rvm.io | bash --ruby

# Install Bundler
gem install bundler

# Go clone any Git repos you are activey working on

# Add these aliases to your ~/.zshrc
alias be="bundle exec "
... 
...


# Install Pods
gem install cocoapods
bundle exec pod install

# Download and install Zoom
https://zoom.us/support/download

# Download and install Slack
https://apps.apple.com/app/slack/id803453959

# Download Twingate VPN for staging access
https://apps.apple.com/us/app/twingate/id1501592214

# Setup Twingate
https://github.com/StartEngine/Twingate_GroupPolicyEditor
- Get API token from Cameron OR Devender

# Setup git aliases in ~/.gitconfig
[user]
    name = Cameron Ehrlich
    email = cameronehrlich@gmail.com
[alias]
    co = checkout
    br = branch
    ci = commit
    st = status
    unstage = reset HEAD --
[credential]
    helper = osxkeychain
[push]
    default = matching
[filter "lfs"]
    clean = git-lfs clean %f
    smudge = git-lfs smudge %f
    required = true
[core]
    excludesfile = ~/.gitignore_global
[pull]
    rebase = false
    
# Select Xcode version
sudo xcode-select -s /Applications/Xcode.app/Contents/Developer

# Setup mergetool
git config --global diff.tool p4merge
