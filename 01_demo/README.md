
# Introduction to `tmux`

### Manage multiple terminals as you manage multiple windows in your laptop

When working locally, you can manage multiple terminals like any other
program: Using the graphical user interface (GUI) that your OS provides.
You can open, move, and close terminals easily.

When working on the cloud often you don’t have a GUI but only a
terminal.

``` bash
ssh ...
```

Starting a new `tmux` session is like starting your laptop with a fresh
desktop.

``` bash
tmux
```

**All `tmux` commands use the prefix `^b` (Control/Command b).**

You may rename the session.

`^b $`

#### Windows

Creating a new window is like opening a new program-window on your
laptop.

`^b c`

Moving between different terminals is like moving between different
program-windows in your laptop.

`^b #`

You may rename each window.

`^b ,`

Closing a window is like closing a program-window in your laptop.

`^b &`

#### Panels

Splitting a window into panels is like arranging different
program-windows to fit a single screen in your laptop.

`^b %`

Resizing panels is like resizing such program-windows.

`^b ^arrow`

Closing a panel is like closing a program-window.

`^b x`

#### Sessions

Creating a new session is like creating a new virtual desktop on your
laptop.

`^b new`

### Easily detach and re-attach long-running processes from a terminal

Detaching a session is like moving the focus to another vitrual desktop.

`^b d`

``` bash
tmux ls
```

### Work with a remote colleague simultaneously on the same terminal process

A remote colleague may `ssh` into the same server, and attach the same
`tmux` session. This is like collaborating on a google document.

``` bash
ssh ...
```

``` bash
tmux attach -t session-name
```

### Resources

-   <https://tmuxcheatsheet.com/>
