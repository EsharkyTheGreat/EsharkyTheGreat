# Bootstrapping Ubuntu 22.04 LTS

### Configuring Email and Github
Login with emailid into browser
add ssh-key to github using
```
ssh-keygen -t ed25519 -C "EsharkyUbuntu"
cat ~/.ssh/id*.pub
```

### Basic Softwares
- git
- vim
- curl

### Configuring ZSH
```
sudo apt-get install zsh
sh -c "$(curl -fsSL https://raw.githubusercontent.com/ohmyzsh/ohmyzsh/master/tools/install.sh)"
cd ~/.oh-my-zsh/custom/plugins
git clone https://github.com/zsh-users/zsh-autosuggestions.git
git clone https://github.com/zsh-users/zsh-syntax-highlighting.git
cp ~/GitRepos/EsharkyTheGreat/.zshrc ~/.zshrc 
cd ~/GitRepos
git clone https://github.com/dracula/zsh.git
ln -sf /home/eshakry/GitRepos/zsh/dracula.zsh-theme ~/.oh-my-zsh/themes/dracula.zsh-theme
source ~/.zshrc
```

### Setup Caskaydia Font
```
mkdir ~/.local/share/fonts
cd ~/.local/share/fonts
wget https://github.com/ryanoasis/nerd-fonts/releases/download/v2.2.2/CascadiaCode.zip
unzip CascadiaCode.zip
rm CascadiaCode.zip
fc-cache -fv
```

### Setup Rust
```
curl --proto '=https' --tlsv1.2 -sSf https://sh.rustup.rs | sh
```

### Setup TMUX
```
sudo apt install tmux
git clone https://github.com/tmux-plugins/tpm ~/.tmux/plugins/tpm
cp ~/GitRepos/EsharkyTheGreat/.tmux.conf ~/.tmux.conf

```

### Setup Alacritty
```
sudo apt-get install cmake pkg-config libfreetype6-dev libfontconfig1-dev libxcb-xfixes0-dev libxkbcommon-dev python3
git clone https://github.com/alacritty/alacritty.git
rustup override set stable
rustup update stable
cargo build --release
sudo tic -xe alacritty,alacritty-direct extra/alacritty.info
sudo cp target/release/alacritty /usr/local/bin # or anywhere else in $PATH
sudo cp extra/logo/alacritty-term.svg /usr/share/pixmaps/Alacritty.svg
sudo desktop-file-install extra/linux/Alacritty.desktop
sudo update-desktop-database
cp ~/GitRepos/EsharkyTheGreat/.alacritty.yml ~/
```
### Setup VSCode
```
sudo snap install code --classic
```
Get Extensions by settings sync

### Setup Brave Browser
```
sudo snap install brave
```

### Setup Docker
```
Just Follow official Guide
```
#### Images for Docker

### Setup Python
```
sudo apt-get install python3 python3-pip python3.10-venv
```

### Setup Binary Exploitation Tools

### Setup NeoVim

### Setup Discord
```
sudo snap install discord
```
or manually download .deb and
```
sudo dpkg -i ./discord*
```

### Setup Spotify

### Setup Node

### Setup Golang

### Setup C/C++

### Setup Pentesting Tools
```
mkdir ~/Pentesting
mkdir ~/Pentesting/VPNs
sudo apt-get install openvpn
sudo snap install xmind
```
---
# Ricing

