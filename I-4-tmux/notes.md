### TMUX

**Install**
- install tmux
  - sudo apt install tmux
- install tpm (tmux package manager)
  - git clone https://github.com/tmux-plugins/tpm ~/.tmux/plugins/tpm

**Create config**
- create your tmux.conf file in:
  - $HOME/.tmux.conf (OLD)
  - $XDG_CONFIG_HOME/tmux/tmux.conf (MODERN) <- this didn't exist for me
    - this usually equates to $HOME/.config/tmux/tmux.conf
  - touch ~/.config/tmux/tmux.conf
   
**Keywords**
- Session
  - top-most layer of tmux
  - collection of 1+ windows managed as a single unit
  - can have n sessions at any time but typically only attach to one
  - each session has an active window
- Window
  - container to 1+ panes
  - conceptually like tabs in browsers
  - each window as one active pane and you can switch between panes
  - shown at bottom of screen and active is marked with '*'
- Pane
  - splits in the window, represent individual terminal session
  - only one active pane at a time
- prefix
  - how you enter commands into tmux
  - default: ctrl-b
   
**Commands and keybindings**
- create window: prefix + c
  - also sets as current active window for session
- run tmux: tmux
- source tmux config: tmux source YOUR_PATH <- mine is: ~/.config/tmux/tmux.conf
- change window
  - next: prefix n
  - previous: prefix p
  - direct: prefix number (ex: prefix 0)
- swap window: prefix :swap-window -s 2 -t 1 (idk what this does)

**Sources**
- [https://www.youtube.com/watch?v=DzNmUNvnB04](url)
