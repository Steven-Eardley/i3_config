# i3 config

I run two machines, so my desktop computer uses config_dt and my macbook pro 11,1 uses config_mbp. i3 picks
up the right one by using a symbolic link, for example:

	ln -s ~/.i3/config_mbp ~/.i3/config

I've made a few additions to the default config file. Most lines I've added or configured are in sections 
denoted by:

	# -------
	blah settings
	# ------

i3 is awesome. Well, it's not [awesome](http://awesome.naquadah.org/), but it's even better.

## Some instructions:

* It is somewhat optimised for an Apple Wireless Keyboard (config_dt uses eject key on kbd for shutdown).

* To use the status bar configuration, create a symbolic link from i3status.conf, hidden in home folder:
	ln -s ~/.i3/i3status.conf ~/.i3status.conf

* Place i3exit in ~/bin/ and ensure it is executable.

## On macbook:

* Two scripts are included to change the keyboard backlight using the keys. Follow instructions in `kbd_backlight_up`.

* The screen brightness controls require `xbacklight`, installed from `apt`.
