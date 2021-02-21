# My Alacritty Setup

```
brew install --cask alacritty
```

### Require terminfo setup

```
# Clone alacritty
git clone https://github.com/alacritty/alacritty.git
cd alacritty
# setup terminfo
sudo tic -xe alacritty,alacritty-direct extra/alacritty.info
# cleanup
cd .. && rm -rf alacritty

```

### Tmux and Vim Italic Comment

```
~/.tmux.conf
# Add true color & italics support with alacritty terminal
set -g default-terminal "alacritty"

~/.vimrc
" Enable italics, Make sure this is immediately after colorscheme
" https://stackoverflow.com/questions/3494435/vimrc-make-comments-italic
highlight Comment cterm=italic gui=italic

```

# Thank you
