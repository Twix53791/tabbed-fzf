# tabbed-fzf
An integration of fzf into suckless tabbed, spawning fzf as a new tab, to use it as a 'file picker', 'app picker' or whatever you want...
It is writed for an bspwm environment, with ranger rifle.

# Install & run
Add this script to /usr/local/bin and use it like that: tabbed -r 2 -s st -w '' -e tabbed-fzf.
You can also put the script anywhere else, and so use rather: tabbed -r 2 -s st -w '' -e bash -c '/path-to-this-script'.
If you don't want to use `st` as a terminal to launch the script in tabbed, use another compatible terminal, cf. tabbed man page.

# Dependencies
- [`tabapp`](https://github.com/Twix53791/bsp-tabapp)
- `rifle` cf. [ranger](https://github.com/ranger/ranger)
- `bspwm`
- `tabbed` can be installed from the [suckless site](https://tools.suckless.org/tabbed/) or from the AUR repository ; it is recommanded to install tabbed-git then. But if you want a patched tabbed : or your arrive to patch it succesfully (which is not my case), or you find a fortunate git hub repo implementing your wanted patches. There is plenty. Personnaly, I use only the hidetabs patch, from [this repo](https://github.com/hXtreme/suckless-tabbed). Just git clone, then, as root is something if wrong, make clean install as the read.me advise.

You coud probably replace rifle by something else, like xdg-open, and also rewrite the script to make it work outside bspwm.

