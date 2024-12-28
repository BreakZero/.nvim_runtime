### Setup
#### 1. Install Neovim via Homebrew
To install Neovim, run the following command:
```shell
brew install neovim
```
#### 2. Download the Configuration
Get the default Neovim configuration by running:
```shell
mkdir -p ~/.config/nvim
curl -o ~/.config/nvim/init.vim https://raw.githubusercontent.com/BreakZero/.nvim_runtime/main/nvim/init.vim
```
#### 3. Install vim-plug Plugin Manager
To install the `vim-plug` plugin manager, run:
```shell
sh -c 'curl -fLo "${XDG_DATA_HOME:-$HOME/.local/share}"/nvim/site/autoload/plug.vim --create-dirs \
       https://raw.githubusercontent.com/junegunn/vim-plug/master/plug.vim'
```
#### 4. Initialize Plugins in Neovim
After starting Neovim, install the plugins by running the following command:
```vim
:PlugInstall
```

### Others

#### Replace vim with nvim
If you want to use nvim as a replacement for vim, follow these steps:
1. Open your ~/.zshrc file:
```shell
nano ~/.zshrc
```
2. Add the following line:
```shell
alias vim="nvim"
```
3. Save the file and apply the changes by running:
```shell
source ~/.zshrc
```

#### Set nvim as the default Git editor
To configure nvim as Git’s default editor, follow these steps:

1. Set the Git editor path:
```shell
git config --global core.editor "{nvim_path}"
```
Replace {nvim_path} with the full path to your nvim executable. For example:
```shell
git config --global core.editor "/usr/bin/nvim"
```
2. Verify the configuration:
```shell
git config --global core.editor
```
This should output the path to nvim.
