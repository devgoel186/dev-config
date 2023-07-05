# TMUX Custom Config for Power User

A custom tmux configuration (including theming and status bar) and tmux launch script for boosted productivity that comprises of tmux setup with three different windows for the most basic daily tasks you do on your system.

## TMUX Configuration

The TMUX configuration file `.tmux.conf` provides the following changes in the basic tmux layout:
- Set prefix as C-a
- Set vim key-binding for navigation between panes
- Set `<prefix>-C-[` and `<prefix>-C-]` for splitting panes horizontally and vertically respectively
- Enable mouse control
- Change status bar position to top
- Use multiple plugins from [dracula/tmux](https://github.com/dracula/tmux) that are displayed in the status bar

## Custom TMUX Layout Launch Script

### TMUX Windows

The script `dev-tmux` launches a tmux session by the name of `dev`, with the following three starting windows:
- 'vim'
- 'explorer'
- 'processes'

### Utilities
- [nvim](https://github.com/neovim/neovim)
- [ranger](https://github.com/ranger/ranger)
- [btop](https://github.com/aristocratos/btop)

### Installation and Setup
Install the utilities mentioned in [Utilities](#Utilities) with your system's package manager.
Then, from the directory where you download the script `dev-tmux`, execute the following commands:

```
sudo cp dev-tmux /usr/local/bin/
sudo chmod +x dev-tmux
```
This will make the script executable from anywhere in your filesystem (provided that /usr/local/bin/ is included in your $PATH).

### Future Scope
This is a very short script that I personally use for my daily development. The empty panes that are created can be used to connect to ssh sessions, refer to man pages, or get that sweet-old `neofetch` out to flex your hardware.
The script is customizable, and can be modified to include anything you wish in your tmux setup.
