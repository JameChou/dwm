## dwm - dynamic window manager
============================
dwm is an extremely fast, small, and dynamic window manager for X.


### Requirements
------------
In order to build dwm you need the Xlib header files.

#### ArchLinux
```bash
sudo pacman -S xorg xorg-init
```

### Installation


#### Source Code & Install
```bash
# Please make sure you already installed the git make gcc g++.
sudo pacman -S git make gcc g++ # On ArchLinux system.
sudo apt-get install git make gcc g++ # On Debian distribution.
sudo yum install git make gcc g++ # On Fedora distribution.


# Clone dwm source from suckless official git repository.
git clone https://git.suckless.org/dwm

cd dwm 
sudo make clean install
```

#### xorg
Please make sure you already installed Xorg. If you have done that, read next section.


```bash
# On ArchLinxu.
sudo pacman -S xorg xorg-init

cp /etc/X11/xinit/xinitrc ~/.xinitrc

# Start dwm when startx.
echo `exec dwm` >> ~/.xinitrc
```

#### Pathes

![dwm-alpha-20201019-61bb8b2.diff](https://dwm.suckless.org/patches/alpha/)
![dwm-autostart-20161205-bb3bd6f.diff](https://dwm.suckless.org/patches/autostart/)
![dwm-fancybar-20220527-d3f93c7.diff](https://dwm.suckless.org/patches/fancybar/)
![dwm-fullgaps-toggle-20200830.diff](https://dwm.suckless.org/patches/fullgaps/)
![dwm-gaplessgrid-20160731-56a31dc.diff](https://dwm.suckless.org/patches/gaplessgrid/)
![dwm-pertag-6.2.diff](https://dwm.suckless.org/patches/pertag/)
![dwm-restartsig-20180523-6.2.diff](https://dwm.suckless.org/patches/restartsig/)
![dwm-scratchpad-6.2.diff](https://dwm.suckless.org/patches/scratchpads/)
