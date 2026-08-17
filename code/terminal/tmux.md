# TMUX

## Prefix Keys

I have 3 prefix keys configured (all equivalent):

| Key          | Keyboard | Notes                                               |
|:------------:|:--------:|:----------------------------------------------------|
| `Ctrl+Space` | All      | Primary prefix                                      |
| `` ` ``      | QWERTY   | Key next to 1 (press twice to type literal `` ` ``) |
| `œ`          | AZERTY   | Key next to 1 (press twice to type literal `œ`)     |

## Shortcuts

### Sessions

| Action                      | Shortcut                        |
|:----------------------------|:--------------------------------|
| Create new session          | `tmux new -s <name>`            |
| Create or attach to session | `tmux new-session -A -s <name>` |
| Rename session              | `<prefix> + $`                  |
| Detach from session         | `<prefix> + d`                  |
| List all sessions           | `<prefix> + s`                  |
| Session and window preview  | `<prefix> + w`                  |
| Previous session            | `<prefix> + (`                  |
| Next session                | `<prefix> + )`                  |
| Attach to last session      | `tmux attach` or `tmux a`       |
| Attach to named session     | `tmux attach -t <name>`         |
| Kill session                | `tmux kill-session -t <name>`   |

### Windows

| Action                     | Shortcut         |
|:---------------------------|:-----------------|
| Create window              | `<prefix> + c`   |
| Rename current window      | `<prefix> + ,`   |
| Close current window       | `<prefix> + &`   |
| List windows               | `<prefix> + w`   |
| Previous window            | `<prefix> + p`   |
| Next window                | `<prefix> + n`   |
| Switch to window by number | `<prefix> + 0-9` |
| Toggle last active window  | `<prefix> + l`   |

### Panes

| Action                          | Shortcut                |
|:--------------------------------|:------------------------|
| Split vertically (pane right)   | `<prefix> + \|`         |
| Split horizontally (pane below) | `<prefix> + -`          |
| Toggle last active pane         | `<prefix> + ;`          |
| Switch to pane (direction)      | `<prefix> + arrow keys` |
| Show pane numbers               | `<prefix> + q`          |
| Switch to pane by number        | `<prefix> + q + 0-9`    |
| Toggle pane zoom                | `<prefix> + z`          |
| Close current pane              | `<prefix> + x`          |
| Convert pane to window          | `<prefix> + !`          |

### Custom Bindings (from my config)

| Action                      | Shortcut            |
|:----------------------------|:--------------------|
| Reload tmux config          | `<prefix> + r`      |
| Copy to system clipboard    | `<prefix> + Ctrl+c` |
| Paste from system clipboard | `<prefix> + Ctrl+v` |

### Misc

| Action             | Shortcut       |
|:-------------------|:---------------|
| Enter command mode | `<prefix> + :` |
| List key bindings  | `<prefix> + ?` |
| Enter copy mode    | `<prefix> + [` |

## References

- [Tmux Cheat Sheet](https://tmuxcheatsheet.com/)
