# Mac Fresh Install

## Brew

```bash
/bin/bash -c "$(curl -fsSL https://raw.githubusercontent.com/Homebrew/install/HEAD/install.sh)"
# echo 'eval "$(/opt/homebrew/bin/brew shellenv)"' >> ~/.zprofile
eval "$(/opt/homebrew/bin/brew shellenv)"
brew analytics off
```

## Apps

```bash
# remove trash apps from mac, then
brew install --cask yandex-disk
brew install --cask google-chrome
brew install --cask skype
brew install --cask telegram
brew install --cask whatsapp
brew install --cask skim
brew install --cask tunnelblick
brew install --cask transmission
# optional
brew install --cask vlc
brew install --cask zoom
brew install --cask djview
brew install --cask fbreader
brew install --cask balenaetcher
brew install --cask obs
```

# Settings

```bash
brew install rectangle
brew install --cask scroll-reverser # optional

# https://unix.stackexchange.com/a/721052/94655
# cp Cloud/Backup/Settings
# cp .* ~/
# cp LocalDictionary ~/Library/Spelling/
```

## Dev

```bash
xcode-select --install
brew install --cask visual-studio-code
brew install colima
# colima start

# git
brew install git
brew install lazygit

# bash
brew install tldr
brew install tree

# bun
brew tap oven-sh/bun
brew install bun

# Docker
brew install lazydocker

# Nerd fonts
brew tap homebrew/cask-fonts
# brew install font-hack-nerd-font
```

## Passwords

```bash
# encrypt
openssl enc -aes-256-cbc -pbkdf2 -salt -e -in passwords.csv -out passwords.enc -k key
# decrypt
openssl enc -aes-256-cbc -pbkdf2 -d -in passwords.enc -out output.csv -k key
```

## Misc

```bash
brew install --cask utm

# https://www.alpinelinux.org/downloads/ (virt)
modinfo 9p # check
setup-alpine # login root
apk add nnn
vi /etc/fstab
# share /mnt/share 9p trans=virtio 0 0
# /dev/sda3 /mnt/samsung ext4 defaults 0 0
mount -a

# NTFS on MacOS
# https://github.com/osxfuse/osxfuse/wiki/NTFS-3G

# MacOS dev setup
# https://www.chrisatmachine.com/posts/01-macos-developer-setup
```

## Before Reset

```bash
# backup:
1. Vscode settings
2. .dotfiles
3. UTM images
4. VPN configs
5. git push repos
```
