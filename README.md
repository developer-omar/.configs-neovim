# Required Instalations

1. Clone Repository

2. creating symbolic links in home directory

```bash
[~]$ cd "$HOME/.config"
[~]$ ln -s "$HOME/.configs-neovim" nvim
```

3. Install plugin manager [vim-plug](https://github.com/junegunn/vim-plug)

```bash
sh -c 'curl -fLo "${XDG_DATA_HOME:-$HOME/.local/share}"/nvim/site/autoload/plug.vim --create-dirs \
       https://raw.githubusercontent.com/junegunn/vim-plug/master/plug.vim'
```

4. Install [jq](https://github.com/stedolan/jq) for format json string

- Fedora/RHEL/CentOS
```bash
sudo dnf install jq
```

- Ubuntu/Debian
```bash
sudo apt install jq
```

5. Install nodejs>= 14.14 for [Conquer of Completion (Coc)](https://github.com/neoclide/coc.nvim), I suggest install with [Node Version Manager (nvm)](https://github.com/nvm-sh/nvm)

6. For Plugin UltiSnip the Python 3.x interface must be available

# Neovim Configurations

Open Neovim and in command mode

1. install plugins

```
:PlugInstall
```

2. Install coc extensions that you require, example:

```
:CocInstall coc-emmet coc-pairs coc-phpls coc-tsserver coc-html coc-css
```