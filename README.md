# Personal dotfiles
This is my iTerm setup.

## Installation

### Fonts
Right now, I'm using [Nerd fonts](https://github.com/ryanoasis/nerd-fonts). 

```
brew tap caskroom/fonts
brew cask install font-hack-nerd-font
```

### iTerm2 Profile:

1. Copy `iTermProfile.json` to:
```
~/Library/Application Support/iTerm2/DynamicProfiles
```

2. Load Profile called `Michal` in the iTerm2 settings.
3. If iTerm2 doesn't recognize the `Nerd font`, you need to duplicate the `Michal` profile and set the font manually.

### Oh My Zsh
Install the [Oh My Zsh](https://github.com/robbyrussell/oh-my-zsh):
```
sh -c "$(curl -fsSL https://raw.githubusercontent.com/robbyrussell/oh-my-zsh/master/tools/install.sh)"
```

### The `~/.zshrc` profile
1. Copy and paste the content of the `zshrcProfile.sh` to `~/.zshrc`.
2. Update the path to ZSH, so it points to your user:
```bash
export ZSH="/Users/YOUR_USER_GOES_HERE/.oh-my-zsh"
```

### Powerlevel9k
1. Clone the Powerlevel9k to the `~/oh-my-zsh/custom/themes` folder
```
git clone https://github.com/bhilburn/powerlevel9k.git ~/.oh-my-zsh/custom/themes/powerlevel9k
```
### Color LS
[ColorLS](https://github.com/athityakumar/colorls) colorizes the the Terminal's output.
I use it for `lc`  and `ls` commands.
```
gem install colorls
```

### More information

[Nerd Fonts: How to install, configure, and remove programming fonts on a mac](https://medium.com/the-code-review/nerd-fonts-how-to-install-configure-and-remove-programming-fonts-on-a-mac-178833b9daf3)

[Powerlevel9k: personalise your terminal prompt for any programming language](https://medium.com/the-code-review/powerlevel9k-personalise-your-prompt-for-any-programming-language-68974c127c63)

[Lolcat, Colorls, Catpix, and other Ruby Gems to add color to your terminal](https://medium.freecodecamp.org/lolcat-colorls-catpix-and-other-ruby-gems-to-add-color-to-your-terminal-16f4d9499ac7)
