DarK is a monotone icon theme for dark X11 desktops.

![alt text](https://gitlab.com/sixsixfive/dark-icons/raw/master/.preview.png)

### Features:

* Designed to stay in the background, so no disturbing colors
* Recolorable, works even on light themes
* Supports more than 7000 icons from the last decade

Howto install?

## Debian testing/unstable

```
su -c 'apt install fakeroot libfile-fcntllock-perl debhelper findutils --no-install-recommends'
make deb
su -c 'dpkg -i dark-theme_*.deb && apt install -f --no-install-recommends'
```
## SuSE Tumbleweed

```
sudo install fakeroot rpmbuild findutils
make rpm
sudo zypper install --no-recommends dark-icon-theme*.rpm
```

## On other distributions

```
make PREFIX=/usr
```

## FAQ

### What icon themes are included?

* aMule
* DolphinEmu
* FileZilla
* Gajim
* IceWM
* Pidgin
* Scribus
* X11/Freedesktop

### Howto change the Icon-theme color?

Just run the [changecolor.sh](https://gitlab.com/sixsixfive/dark-icons/blob/master/DarK/changecolor.sh) script! eg:

### Icons are unavailable in IceWM

At first you have to create the icon themes with [one of the scripts](https://gitlab.com/sixsixfive/dark-icons/blob/master/DarK/App_themes/icewm_dark):

PS: The icon theme folder must be part of the IconPath key in your preferences file.

PPS: Some themes have internal icons so you can either remove them or replace(eg: symlink or copy) them with the icewm icon folder!
