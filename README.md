# cewm
centi window manager


# what
minimal, yet usable window manager written in shell

# brief overview
wm consists of 3 parts:
* `call` script to send client requests to wm server
* `proxy` script which continuously read wew events and send
  them to server
* `wm` script acting as server. it dispatches requests and
  acts accordingly

# dependencies
- bsd `netcat` (ability to continue after peer disconnect: `-k` option)
- wmutils (both [core](https://github.com/wmutils/core) and [opt](https://github.com/wmutils/opt) for `wew`)
- regular *nix binaries (`car`, `echo`, `sed`, `mkdir`, `touch`, `rm`, etc.)
- `sh`
