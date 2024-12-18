### Setup
#### 1. Install neovim with brew
```sh
brew install neovim
```
#### 2. Clone nvim folder into local
```sh
git clone https://github.com/BreakZero/.nvim_runtime.git ~/.config/nvim
```
#### 3. Install vim-plug
```sh
sh -c 'curl -fLo "${XDG_DATA_HOME:-$HOME/.local/share}"/nvim/site/autoload/plug.vim --create-dirs \
       https://raw.githubusercontent.com/junegunn/vim-plug/master/plug.vim'
```
#### 4. Init Plug for nvim (in nvim)
```vim
:PlugInstall
```
