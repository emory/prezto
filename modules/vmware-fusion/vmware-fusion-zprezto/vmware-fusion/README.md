vmware-fusion
=============

Defines useful(?) [VMWare Fusion][1] aliases.

Settings
--------

Aliases
-------

  - `vmr` attaches or switches to a tmux session.
  - `vml` lists sessions managed by the tmux server.

Caveats
-------

	On Mac OS X, launching tmux can cause the error **launch_msg(...): Socket is not
	connected** to be displayed, which can be fixed by installing
	[reattach-to-user-namespace][3], available in [Homebrew][4], and adding the
	following to *tmux.conf*:
	
    	set-option -g default-command "reattach-to-user-namespace -l $SHELL -l"
	
	Furthermore, tmux is known to cause **kernel panics** on Mac OS X. A discussion
	about this and Prezto has already been [opened][2].
	
Authors
-------

	*The authors of this module should be contacted via the [issue tracker][5].*
	
  	- [Colin Hebert](https://github.com/ColinHebert)
  	- [Georges Discry](https://github.com/gdiscry)
  	- [Xavier Cambar](https://github.com/xcambar)

[1]: http://www.vmware.com/products/fusion
[2]: https://github.com/sorin-ionescu/prezto/issues/62
[3]: https://github.com/ChrisJohnsen/tmux-MacOSX-pasteboard
[5]: https://github.com/sorin-ionescu/prezto/issues
