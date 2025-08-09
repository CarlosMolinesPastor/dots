**TODO for clone my dots**
1. ARCHLINUX
   
   - First, install de packages
    ```bash
    sudo pacman -S git curl wget zsh fzf ripgrep lsd bat starship neovim kitty stow
    ```
    - Dependencies for zsh
    ```bash
    sh -c "$(wget https://raw.githubusercontent.com/ohmyzsh/ohmyzsh/master/tools/install.sh -O -)"
    git clone https://github.com/zsh-users/zsh-syntax-highlighting.git $ZSH_CUSTOM/plugins/zsh-syntax-highlighting
    git clone https://github.com/zsh-users/zsh-autosuggestions ${ZSH_CUSTOM:-~/.oh-my-zsh/custom}/plugins/zsh-autosuggestions
    git clone https://github.com/Aloxaf/fzf-tab ${ZSH_CUSTOM:-~/.oh-my-zsh/custom}/plugins/fzf-tab
    git clone --depth 1 https://github.com/junegunn/fzf.git ~/.fzf
    ~/.fzf/install --key-bindings --completion --no-update-rc
    cd ~
    ```
    - Nerdinstall
    ```bash
    mkdir build
    cd build
    git clone https://github.com/CarlosMolinesPastor/nerdfonts.git
    cd nerdfonts
    chmod +x nerdinstall.sh
    ./nerdinstall.sh
    cd ~
    ```
   - Clone the repository and install
   ```bash
   git clone https://github.com/CarlosMolinesPastor/dots.git
   cd dots
   stow .
   ```
   
   **DISFRUTEN**
