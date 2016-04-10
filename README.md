Older version of libnss for Upwork Team App to work

https://support.upwork.com/hc/en-us/articles/211064108-Linux-troubleshooting-for-Upwork-Team-App#library

To run, execute:

    ./run.sh &

---

Or edit the `.desktop` file to run it from launcher in the future:

Open `/usr/share/applications/upwork.desktop`

Change line:

    Exec=upwork

to:

    Exec=env LD_LIBRARY_PATH=/path/to/upwork-fix/x86_64-linux-gnu upwork
