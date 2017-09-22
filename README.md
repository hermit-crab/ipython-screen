# ipython-screen
Eliminate IPython startup time on Linux by having it run in Screen.
***

Short script that wraps ipython call to be run under GNU Screen terminal multiplexer.

On startup it initializes two IPython sessions: one in foreground and another in background for the next use.

Simply place it into one of your PATH directories or call directly. Accepts IPYTHON_BIN environment variable. Can be run as `ipython-screen -` to only initialize background session (for autostart).

Shortcut install: 
```bash
cd ~/.local/bin && wget https://raw.githubusercontent.com/Unknowny/ipython-screen/master/ipython-screen && chmod +x ipython-screen
```

Useful aliases:
```bash
alias p="IPYTHON_BIN=ipython3 ipython-screen"
alias p2="IPYTHON_BIN=ipython2 ipython-screen"
```
