# My Work Environment 💼🏞️

## zsh (oh-my-zsh)

### zsh - Get It

1. Install zsh
2. Install [oh-my-zsh](https://ohmyz.sh/#install): `sh -c "$(curl -fsSL https://raw.github.com/ohmyzsh/ohmyzsh/master/tools/install.sh)"`

#### Customization

##### Font and Theme

1. [Install Meslo Nerd Font](https://github.com/romkatv/powerlevel10k#meslo-nerd-font-patched-for-powerlevel10k)
2. [Install Powerlevel10k theme](https://github.com/romkatv/powerlevel10k#oh-my-zsh)
3. Optional: use P10K configuration file (place under `~/`) - [.p10k.zsh](.p10k.zsh)

##### Plugins and Other Cool Tools

1. Put in `~/.zshrc`: `plugins=(git colored-man-pages zsh-syntax-highlighting zsh-autosuggestions pip tmux)`
2. [Install fzf](https://github.com/junegunn/fzf)
3. [Install ripgrep](https://github.com/BurntSushi/ripgrep)

Worth taking a look into:
[forgit](https://github.com/wfxr/forgit)

##### zshrc settings

Add the following:

```bash
export LANG=en_IL.UTF-8
export LC_ALL=en_IL.UTF-8
export LC_CTYPE=en_IL.UTF-8
export EDITOR='vim'
export FZF_TMUX=1
export FZF_TMUX_OPTS="-d 40%"
```

### vim

#### vim - Get It

1. Install vim
2. Install [Vundle](https://github.com/VundleVim/Vundle.vim#quick-start) plugin manager
3. Optional: use following vimrc configuration file (place under `~/`) - [.vimrc](.vimrc)

### Tmux

#### Tmux - Get It

1. Install tmux
2. Install Tmux Plugin Manager [tpm](https://github.com/tmux-plugins/tpm)
3. Optional: use following tmux.conf configuration file (place under `~/`) - [.tmux.conf](.tmux.conf)



### VScode

#### VSCode - Get It

Install with pkg manager

##### VScode - Customization

Add the following to user `settings.json`

```json
{
    "terminal.integrated.fontFamily": "MesloLGS NF",
    "files.insertFinalNewline": true,
    "files.trimTrailingWhitespace": true,
    "files.trimFinalNewlines": true,
    "workbench.iconTheme": "vscode-icons",
    "workbench.colorTheme": "One Dark Pro",
    "terminal.integrated.copyOnSelection": true,
    "terminal.integrated.defaultProfile.linux": "code shell",
    "terminal.integrated.profiles.linux": {
        "bash": {
            "path": "bash"
        },
        "zsh": {
            "path": "zsh"
        },
        "fish": {
            "path": "fish"
        },
        "tmux": {
            "path": "tmux",
            "icon": "terminal-tmux"
        },
        "pwsh": {
            "path": "pwsh",
            "icon": "terminal-powershell"
        },
        "code shell": {
            "path": "code-shell",
            "icon": "terminal-tmux",
            "overrideName": true
        }
    },
    "editor.lineNumbers": "relative",
    "terminal.integrated.automationShell.linux": "zsh",
}
```

##### Useful Extensions

Run in terminal:

```bash
echo "ahgood.shift-shift
CoenraadS.bracket-pair-colorizer-2
DavidAnson.vscode-markdownlint
eamodio.gitlens
Gruntfuggly.todo-tree
KevinRose.vsc-python-indent
ms-python.python
ms-python.vscode-pylance
ms-toolsai.jupyter
njpwerner.autodocstring
richie5um2.vscode-sort-json
ryu1kn.partial-diff
streetsidesoftware.code-spell-checker
timonwong.shellcheck
vscode-icons-team.vscode-icons
vscodevim.vim
yzhang.markdown-all-in-one
zhuangtongfa.material-theme" | xargs -L1 code --install-extension

```



### Python

#### Pylint

1. [Pylint](https://pypi.org/project/pylint/)
2. [Pylint-Venv](https://pypi.org/project/pylint-venv/)
