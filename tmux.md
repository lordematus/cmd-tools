# Tmux cheatsheet

## Basics

- Starting tmux: `$ tmux`
- Closing session: `$ exit`
- PREFIX: `Ctrl+b`
- Get a list of keybindings and command: `PREFIX` + `?`

### Sessions

- Creating session without name: `$ tmux new-session`
- Creating named sessions: `$ tmux new-session -s session_name` (or `tmux new -s session_name`)
- Creating named session in the background: `$ tmux new -s session_name -d`
- List existing sessions: `$ tmux list-sessions` (or `tmux ls`)
- Attach session: `$ tmux attach -t session_name`
- Kill sessions: `$ tmux kill-session -t session_name`
- Detach session: `PREFIX` + `d`

### Windows

- Create named session with a named window: `$ tmux new -s session_name -n window_name`
- Create a window in the current session: Press `PREFIX` + `c`
- Rename the current window: Press `PREFIX` + `,`
- Switch to the Next window: Press `PREFIX` + `n`
- Switch to the Previous window: Press `PREFIX` + `p`
- Switch to window [0-9]: Press `PREFIX` + `[0-9]`
- Close a window: Press `PREFIX` + `&` (exit also works)

### Panes

- Divide in half vertically: Press `PREFIX` + `%`
- Divide in half horizontally: Press `PREFIX` + `"`
- Cycle through the panes: Press `PREFIX` + `o` (`PREFIX` + `UP/DOWN/LEFT/RIGHT` also works)
- Cycle through the pane layouts: Press `PREFIX` + `SPACEBAR`
- Closing panes: Press `PREFIX` + `x`
- Momentarily displays pane numbers in each pane: `PREFIX` + `q`

### Command mode

- Enter the command mode: Press `PREFIX` + `:`

(Example) Create a new window and execute a command: `new-window -n window_name "command"`

## Configuring Tmux

In progress...
