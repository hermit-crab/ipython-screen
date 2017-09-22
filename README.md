# ipython-screen
Eliminate IPython startup time on Linux by having it run in Screen.
***

Short script that wraps ipython call to be run under GNU Screen terminal multiplexer.

On startup it initializes two ipython sessions: one in foreground and another in background for the next use.

Simply place it into one of your PATH directories or call directly.

Accepts IPYTHON_BIN environment variable. Use `ipython-screen -` to only initialize background session (for autostart).


Useful aliases:
```bash
alias p="IPYTHON_BIN=ipython3 ipython-screen"
alias p2="IPYTHON_BIN=ipython2 ipython-screen"
```
