##dminiwm.multiview
### it's minimal and dynamic

I started this from catwm 31/12/10 ( https://bbs.archlinux.org/viewtopic.php?id=100215&p=1 )
    See dminiwm.c or config.h for thanks and licensing.
Screenshots and ramblings/updates at https://bbs.archlinux.org/viewtopic.php?id=126463


###Summary
-------


**dminiwm.multiview** is a very minimal and lightweight dynamic tiling window manager.

>    Start your X session with the appropriate xrandr commands

>    and the window manager places different desktops on each screen

>    I will try to stay under 1000 SLOC.

>    Currently under 980 lines with the config file included.


###Modes
-----

It allows the "normal" method of tiling window managers(with the new window as the master)
    or with the new window opened at the bottom or the top of the stack.

 *There's vertical tiling mode:*

    --------------
    |        | W |
    |        |___|
    | Master |   |
    |        |___|
    |        |   |
    --------------

 *Horizontal tiling mode:*

    -------------
    |           |
    |  Master   |
    |-----------|
    | W |   |   |
    -------------
    
 *Grid tiling mode:*

    -------------
    |      | W  |
    |Master|    |
    |------|----|
    |      |    |
    -------------

 *Fullscreen mode*(which you'll know when you see it)

 All accessible with keyboard shortcuts defined in the config.h file.
 
 * The window *W* at the top of the stack can be resized on a per desktop basis.
 * Changing a tiling mode or window size on one desktop doesn't affect the other desktops.


###Recent Changes
--------------

2/4/12

>	Added multi monitor support

###Status
------

There are more options in the config file than the original catwm.

  * 
  * 
  * 
  * 
  * 
  * 
  * 
  * 
  * 
  * 
  * 
  * 


###Installation
------------

Need Xlib, then:

edit the config.h.def file to suit your needs
and save it as config.h.

    $ make
    # make install
    $ make clean

Add the appropriate commands to *e.g.* xinitrc to start the xsession
 with the monitors where you want them

    *e.g.*

    xrandr --output LVDS1 --mode 1366x768
    xrandr --output VGA1 --mode 1280x1024 --right-of LVDS1

###Bugs
----

[ * No bugs for the moment ;) (I mean, no importants bugs ;)]


###Todo
----

  * 

