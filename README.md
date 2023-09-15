# Using WSL

``` powershell
# Instalar WSL
wsl --install -d Ubuntu
```

# My Ubuntu

``` sh

# verifica se hpa atualizações
sudo apt update
apt list --upgradable

# atualizar o sistema
sudo apt upgrade

# Installing zsh
sudo apt install zsh

# Makes zsh as shell default
chsh -s $(which zsh)

# abrir nova aba Ubuntu
# Escolher opção 2

# Installing curl
sudo apt install curl

# Installing oh-my-zsh
sh -c "$(curl -fsSL https://raw.githubusercontent.com/ohmyzsh/ohmyzsh/master/tools/install.sh)"

# Installing zsh-syntax-highlight
git clone https://github.com/zsh-users/zsh-syntax-highlighting.git ${ZSH_CUSTOM:-~/.oh-my-zsh/custom}/plugins/zsh-syntax-highlighting

# Install powerlevel10k
git clone --depth=1 https://github.com/romkatv/powerlevel10k.git ${ZSH_CUSTOM:-$HOME/.oh-my-zsh/custom}/themes/powerlevel10k

# Installing colorls
sudo apt install build-essential
sudo apt install ruby-full
sudo gem install colorls

# Installing nvm (node version manager)
curl -o- https://raw.githubusercontent.com/nvm-sh/nvm/v0.39.5/install.sh | bash

# Installing NodeJS (LTS)
nvm install --lts

# Setup Clone
git clone https://github.com/Camille846/myUbuntu.git ~/.dotfiles
cd ~/.dotfiles
ln -s ~/.dotfiles/.gitconfig ~/.gitconfig
ln -s ~/.dotfiles/.p10k.zsh ~/.p10k.zsh
ln -s ~/.dotfiles/.zshrc ~/.zshrc

```
