# indicator-crystalhd

This is an indicator for Broadcom Crystal HD adapter altered to run with the latest updated driver from https://github.com/dbason/crystalhd (an active fork of https://github.com/yeradis/crystalhd).

This indicator was last tested with Cinnamon in Mint 18.1 x64 and ran just fine.

~~Due to the updated driver, I could not find a way to determine whether it's working (decoding) or not. But at least you can switch on and off using this updated indicator.~~

The indicator should now correctly display whether the Crystal HD adapter is being used for decoding (indicator turns blue) or not (indicator turns white). With a right click, the indicator can also be used to enable or disable the crystalhd kernel module.

--------

It's an indicator for Ubuntu's Unity, but is also usable with LXDE, Xfce e.g.

The indicator shows several states of the crystalhd (Broadcom BCM70012 BCM70015) linux driver: Disabled, enabled, working, stalling and erroneous. It also lets you disable and enable the driver.

**Ubuntu Unity:**

![1](http://i.imgur.com/pKjWmZt.png) 

![2](http://i.imgur.com/BAnJK4t.png)

![3](http://i.imgur.com/PEKLpDN.png)

**Xfce ,LXDE, Openbox(tint2):**

![4](http://i.imgur.com/72C9QmN.png)

![5](http://i.imgur.com/aM3TjAm.png)

![6](http://i.imgur.com/tfjaPf3.png)



##Installation

* Clone or download the repository
* cd into the repository and run this command (you may need to ``sudo apt install checkinstall``): 
```shell
chmod 755 usr/bin/indicator-crystalhd
sudo checkinstall cp -R usr /
```
* Run `sudo indicator-crystalhd` at the terminal. It'll run and set itself to run at autostart.

--------

~~It only works with version v3.10.0 (0.9.30) of the driver. Here is a short tutorial on how to install the latest v3.10.0 (0.9.30) crystalhd driver: http://code.google.com/p/indicator-crystalhd/wiki/CrystalHDHowTo ~~

~~When the driver is running fine, it is possible to use the indicator. You can download it here: http://indicator-crystalhd.googlecode.com/files/indicator-crystalhd-1.24.tar.gz  ~~

~~I've altered the code to work with latest updated driver from https://github.com/yeradis/crystalhd . I can run this indicator just fine in Ubuntu-Mate 14.14 x64.~~

**EZ 2017-05-13** I've altered the code to work with latest updated driver from https://github.com/dbason/crystalhd (an active fork of https://github.com/yeradis/crystalhd). I can run this indicator just fine in Mint 18.1 x64 (cinnamon).

*** If you are looking for the original script, if the link above fails, you can download at https://github.com/Ardakilic/indicator-crystalhd/tree/02127772123e34023c8b2a11d6ea264a6aecd15d ***

Instructions are in the README file. Python-appindicator is needed (already included in Ubuntu)
