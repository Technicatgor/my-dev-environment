# My Dev Environment

## Homebrew

Ref Link: https://brew.sh/

```bash
/bin/bash -c "$(curl -fsSL https://raw.githubusercontent.com/Homebrew/install/HEAD/install.sh)"
```

## Terminal Setup

- [warp](https://www.warp.dev/): `brew install --cask warp`

- ohmyzsh - [.zshrc](./.zshrc) shell configuration
  `sh -c "$(curl -fsSL https://raw.githubusercontent.com/ohmyzsh/ohmyzsh/master/tools/install.sh)"`

- p10k
  `git clone --depth=1 https://github.com/romkatv/powerlevel10k.git ~/.oh-my-zsh/themes/powerlevel10k`

## LazyVim

- neovim [installation](https://technicatgor.github.io/posts/LazyVimIDE/)
  `brew install neovim`
- [nvim](./nvim/) configuration and plugin

## LazyGit

- installation:

```bash
LAZYGIT_VERSION=$(curl -s "https://api.github.com/repos/jesseduffield/lazygit/releases/latest" | grep -Po '"tag_name": "v\K[^"]*')
curl -Lo lazygit.tar.gz "https://github.com/jesseduffield/lazygit/releases/latest/download/lazygit_${LAZYGIT_VERSION}_Linux_x86_64.tar.gz"
tar xf lazygit.tar.gz lazygit
sudo install lazygit /usr/local/bin
```

## Sketchybar

Repo: https://github.com/FelixKratz/SketchyBar

### Setup Requires

- sketchybar: `brew tap FelixKratz/formulae` and `brew install sketchybar`
- jq (json command line processor): `brew install jq`
- SF Pro Font: `brew tap homebrew/cask-fonts` and `brew install font-sf-pro`
- SF Symbols: `brew install --cask sf-symbols`
- Sketchybar App Font:

```bash
`curl -L https://github.com/kvndrsslr/sketchybar-app-font/releases/download/v1.0.16/sketchybar-app-font.ttf -o $HOME/Library/Fonts/sketchybar-app-font.ttf`
```

### Relevant Files

- [.config/sketchybar](.config/sketchybar/)
