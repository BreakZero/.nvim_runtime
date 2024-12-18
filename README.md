### Setup
1. Install neovim with brew
> brew install neovim
2. Clone nvim folder into local
> git clone https://github.com/BreakZero/.nvim_runtime.git ~/.config/nvim
3. Install vim-plug
> sh -c 'curl -fLo "${XDG_DATA_HOME:-$HOME/.local/share}"/nvim/site/autoload/plug.vim --create-dirs \
>       https://raw.githubusercontent.com/junegunn/vim-plug/master/plug.vim'
4. Init Plug for nvim
> :PlugInstall (in nvim)