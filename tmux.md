# tmux cheatsheet

### Reload tmux conf

```
source ~/.tmux.conf - from within tmux
tmux source ~/.tmux.conf - from terminal
```

### Management 


```
tmux - start new
tmux new -s myname - start new with session name:
tmux a  # - or at, or attach
tmux a -t myname - attach to named
tmux ls - list sessions
tmux kill-session -t myname - kill session
killall tmux - kill all the tmux sessions
tmux ls | grep : | cut -d. -f1 | awk '{print substr($1, 0, length($1)-1)}' | xargs kill - kill all the tmux sessions
```

### Sessions

In tmux, hit the prefix `ctrl+b` and then:

```
:new<CR> - new session
s - list sessions
$ - name session
```

### Windows (tabs)

```
c - new window
w - list windows
f - find window
, - name window
& - kill window
t - show time
````

### Panes (splits) 

```
% - vertical split
" - horizontal split
q - show pane numbers
& - kill pane
s - break pane into another window
j - restore pane from window
⍽ - space - toggle between layouts
q - Show pane numbers, when the numbers show up type the key to goto that pane
{ - Move the current pane left
} - Move the current pane right
z - toggle pane zoom
```
