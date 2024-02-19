# st
### personal build

![st demo](static/demo.png)

#### patches:
	- st-anysize-20220718-baa9357.diff
	- st-dracula-0.8.5.diff
	- st-scrollback-0.8.5.diff
	- st-scrollback-mouse-20220127-2c5edf2.diff
	- st-scrollback-mouse-altscreen-20220127-2c5edf2.diff
	- st-scrollback-mouse-increment-0.8.2.diff
	- st-scrollback-reflow-0.8.5.diff
	- st-w3m-0.8.3.diff

st - simple terminal
--------------------
st is a simple terminal emulator for X which sucks less.


Requirements
------------
In order to build st you need the Xlib header files.


Installation
------------
Edit config.mk to match your local setup (st is installed into
the /usr/local namespace by default).

Afterwards enter the following command to build and install st (if
necessary as root):

    make clean install


Running st
----------
If you did not install st with make clean install, you must compile
the st terminfo entry with the following command:

    tic -sx st.info

See the man page for additional details.

Credits
-------
Based on Aurélien APTEL <aurelien dot aptel at gmail dot com> bt source code.

