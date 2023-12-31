# This includes almost all packages i install on my desktop.

## 1. Office 
1. There are many of office utilities. Heres a [list](https://wiki.archlinux.org/title/Category:Office)
2. In my daily usage i prefer [LibreOfiice](https://wiki.archlinux.org/title/LibreOffice).
~~~
$ sudo pacman -S libreoffice-fresh
~~~
There are two libreoffice -
  * [libreoffice-still](https://archlinux.org/packages/?name=libreoffice-still) is the stable maintenance branch with relatively rare updates, for conservative users.
  * [libreoffice-fresh](https://archlinux.org/packages/?name=libreoffice-fresh) is the feature branch, with new program enhancements for early adopters or power users.

## 2. Browsers
1. There are many web browsers. Heres the [list](https://wiki.archlinux.org/title/List_of_applications/Internet#Web_browsers).
2. My Go-To for now are firefox and brave. Firefox for daily. Sometimes and idk why some websites dont work on firefox so brave.
~~~
$ sudo pacman -S firefox
$ yay -S brave-bin             // If you wanna compile it you can use brave-git or brave.
~~~
3. if you wanna install tor use
```
$ sudo pacman -S torbrowser-launcher
```
### I got a cool list on privacy status of stuff like browsers, web engines, etc. [Spyware Watchdog Article Catalog](https://xgqt.gitlab.io/spywarewatchdog/articles/index.html)

## 3. Audio Player
I dont generally use any app for local music as i dont have them because i'm lazy to download and play them. Maybe i'll do if i make my own server but for now i use web versions of spotify or spotify desktop. Install [spotify-launcher](https://archlinux.org/packages/?name=spotify-launcher). This package manages a per-user installation in your home directory, allowing Spotify to update itself independently of pacman (similar to how Spotify self-updates on other operating systems).
~~~
$ sudo pacman -S spotify-launcher
~~~

If you prefer to manage Spotify updates with pacman, instead use [spotify](https://aur.archlinux.org/packages/spotify) from AUR which repackages [Spotify for Linux](https://www.spotify.com/us/download/linux/). If you need to add and play local files you need to additionally install [zenity](https://archlinux.org/packages/?name=zenity) and [ffmpeg4.4](https://archlinux.org/packages/?name=ffmpeg4.4). 
~~~
$ yay -S spotify
$ sudo pacman -S zenity ffmpeg4.4
~~~
If you wanna use third-party clients to use spotify check [wiki](https://wiki.archlinux.org/title/spotify). I have only used [spotify-tui](https://github.com/Rigellute/spotify-tui). its really cool. **You'll need spotify premium accounts to use the third party clients**.
If you looking for more multimedia utilities. go to the [wiki](https://wiki.archlinux.org/title/List_of_applications/Multimedia)

## 4. PDF
I use Master PDF editor and okular(viewer). There are many others if you wanna [explore](https://wiki.archlinux.org/title/PDF,_PS_and_DjVu)
~~~
$ yay -S masterpdfeditor okular
~~~

## 5. torrenting client
My go to is [qbittorrent](https://wiki.archlinux.org/title/QBittorrent)
~~~
$ sudo pacman -S qbittorrent
~~~

## 6. Discord
~~~
$ sudo pacman -S discord
~~~

## 7. OBS Studio
~~~
$ sudo pacman -S obs-studio
~~~

## 8. File manager
There are various [file managers](https://wiki.archlinux.org/title/Category:File_managers). I prefer to use thunar.
~~~
$ sudo pacman -S thunar
~~~

## 9. Raster Graphic editors
I just use [Gimp](https://wiki.archlinux.org/title/GIMP). There are various other [editors](https://wiki.archlinux.org/title/List_of_applications/Multimedia#Raster_graphics_editors).
~~~
$ sudo pacman -S gimp
~~~

## 10. [Obsidian](https://obsidian.md/)
~~~
$ sudo pacman -S obsidian
~~~

## 11. Media player
I use [vlc](https://wiki.archlinux.org/title/VLC_media_player). If you wanna see other [options](https://wiki.archlinux.org/title/List_of_applications/Multimedia#Video)
~~~
$ sudo pacman -S vlc
~~~

## 12. Text editor
For now its Neovim. I use these [dotfiles](https://github.com/QuantiniumX/nvim-.dotfiles). For other text [editors](https://wiki.archlinux.org/title/Category:Text_editors)
~~~
$ sudo pacman -S neovim
~~~

## 13. [VSCode](https://wiki.archlinux.org/title/Visual_Studio_Code)
There are three different packages.
~~~
$ sudo pacman -S code   // Official Arch Linux open-source release. Ships a configuration enabling Open VSX.
$ yay -S  visual-studio-code-bin      // Proprietary Microsoft-branded release.
$ yay -S vscodium       //Community open-source release. Nullifies telemetry in the source code [1], also ships configuration with Open VSX.
~~~
