# CTF Challenge: printing_exported_variable

## Table of Content

- commands-executed: env
- flag :pwn.college{E7C3ZA0jdeOrjeaHxEZ8-lEa44_.dhTN1QDLzETN0czW}


### Output:
```console

hacker@variables~printing-exported-variables:~$ env
SHELL=/run/dojo/bin/bash
SESSION_MANAGER=local/variables~printing-exported-variables:@/tmp/.ICE-unix/116,unix/variables~printing-exported-variables:/tmp/.ICE-unix/116
WINDOWID=27262979
COLORTERM=truecolor
XDG_CONFIG_DIRS=/run/dojo/etc/xdg:/etc/xdg
HOSTNAME=variables~printing-exported-variables
SSH_AUTH_SOCK=/tmp/ssh-XXXXXXpGi1qi/agent.133
SSH_AGENT_PID=134
GDK_PIXBUF_MODULE_FILE=/nix/store/gpiy256schil984zxxqx8y0d4q2j6bm8-librsvg-2.58.1/lib/gdk-pixbuf-2.0/2.10.0/loaders.cache
PWD=/home/hacker
PANEL_GDK_CORE_DEVICE_EVENTS=0
DOJO_AUTH_TOKEN=9700ad469d07716992e51780021746c4e1d1afe9e2b2a4f1907463ae6a97b348
GI_TYPELIB_PATH=/nix/store/fhv964af9qiyvipfzxh53pgln1r18za6-glib-2.80.2/lib/girepository-1.0:/nix/store/aps6xk6z2zwdl3kjh1ckc30nz47k773b-at-spi2-core-2.52.0/lib/girepository-1.0:/nix/store/yg53p80khxl4v5r070a0mff7h34i29wj-gdk-pixbuf-2.42.12/lib/girepository-1.0:/nix/store/szyhy2fbbm1318qrkl6p4j5ibx6xykl4-gsettings-desktop-schemas-46.0/lib/girepository-1.0:/nix/store/97yyz3qlzi69hr9r71b4v2ld0d2djf4g-harfbuzz-8.4.0/lib/girepository-1.0:/nix/store/f2vnqb6i9bi5jdhdb708rpmf0pry6iqn-pango-1.52.2/lib/girepository-1.0:/nix/store/mlzl5gqfnbvrpy44zd2d5zdv1r04x977-gtk+3-3.24.43/lib/girepository-1.0:/nix/store/gpiy256schil984zxxqx8y0d4q2j6bm8-librsvg-2.58.1/lib/girepository-1.0:/nix/store/gxkkwrp9bwykw0c4mzlcd5fl15j23dir-gobject-introspection-wrapped-1.80.1/lib/girepository-1.0:/nix/store/x0kxca5lxm75sbnalymi4xc338q8a5bn-gobject-introspection-1.80.1/lib/girepository-1.0:/nix/store/klav9wwvb3xnvgqrc8v367j6qfrvlfii-garcon-4.18.2/lib/girepository-1.0:/nix/store/x6ypmj6lb201js4s09mz29zzzpac8avm-libdbusmenu-gtk3-16.04.0/lib/girepository-1.0:/nix/store/6f7icflqwjf8hap93dv01r3rng5i5ghh-libxfce4util-4.18.2/lib/girepository-1.0:/nix/store/snq35d3kv7ms1xajigwvsyzwm0k3rlpz-libxfce4ui-4.18.6/lib/girepository-1.0:/nix/store/s1207g605rq4mh3i86m6l4242frq6fiq-libwnck-43.0/lib/girepository-1.0:/nix/store/3zi7zn2bbz3jpx8ds4nharz67j6ajp9k-xfconf-4.18.3/lib/girepository-1.0:/nix/store/xpgf309sv9w5majf26zg50fpd9vqk1x3-xfce4-panel-4.18.6/lib/girepository-1.0
HOME=/home/hacker
LANG=C.UTF-8
LS_COLORS=rs=0:di=01;34:ln=01;36:mh=00:pi=40;33:so=01;35:do=01;35:bd=40;33;01:cd=40;33;01:or=40;31;01:mi=00:su=37;41:sg=30;43:ca=00:tw=30;42:ow=34;42:st=37;44:ex=01;32:*.7z=01;31:*.ace=01;31:*.alz=01;31:*.apk=01;31:*.arc=01;31:*.arj=01;31:*.bz=01;31:*.bz2=01;31:*.cab=01;31:*.cpio=01;31:*.crate=01;31:*.deb=01;31:*.drpm=01;31:*.dwm=01;31:*.dz=01;31:*.ear=01;31:*.egg=01;31:*.esd=01;31:*.gz=01;31:*.jar=01;31:*.lha=01;31:*.lrz=01;31:*.lz=01;31:*.lz4=01;31:*.lzh=01;31:*.lzma=01;31:*.lzo=01;31:*.pyz=01;31:*.rar=01;31:*.rpm=01;31:*.rz=01;31:*.sar=01;31:*.swm=01;31:*.t7z=01;31:*.tar=01;31:*.taz=01;31:*.tbz=01;31:*.tbz2=01;31:*.tgz=01;31:*.tlz=01;31:*.txz=01;31:*.tz=01;31:*.tzo=01;31:*.tzst=01;31:*.udeb=01;31:*.war=01;31:*.whl=01;31:*.wim=01;31:*.xz=01;31:*.z=01;31:*.zip=01;31:*.zoo=01;31:*.zst=01;31:*.avif=01;35:*.jpg=01;35:*.jpeg=01;35:*.mjpg=01;35:*.mjpeg=01;35:*.gif=01;35:*.bmp=01;35:*.pbm=01;35:*.pgm=01;35:*.ppm=01;35:*.tga=01;35:*.xbm=01;35:*.xpm=01;35:*.tif=01;35:*.tiff=01;35:*.png=01;35:*.svg=01;35:*.svgz=01;35:*.mng=01;35:*.pcx=01;35:*.mov=01;35:*.mpg=01;35:*.mpeg=01;35:*.m2v=01;35:*.mkv=01;35:*.webm=01;35:*.webp=01;35:*.ogm=01;35:*.mp4=01;35:*.m4v=01;35:*.mp4v=01;35:*.vob=01;35:*.qt=01;35:*.nuv=01;35:*.wmv=01;35:*.asf=01;35:*.rm=01;35:*.rmvb=01;35:*.flc=01;35:*.avi=01;35:*.fli=01;35:*.flv=01;35:*.gl=01;35:*.dl=01;35:*.xcf=01;35:*.xwd=01;35:*.yuv=01;35:*.cgm=01;35:*.emf=01;35:*.ogv=01;35:*.ogx=01;35:*.aac=00;36:*.au=00;36:*.flac=00;36:*.m4a=00;36:*.mid=00;36:*.midi=00;36:*.mka=00;36:*.mp3=00;36:*.mpc=00;36:*.ogg=00;36:*.ra=00;36:*.wav=00;36:*.oga=00;36:*.opus=00;36:*.spx=00;36:*.xspf=00;36:*~=00;90:*#=00;90:*.bak=00;90:*.crdownload=00;90:*.dpkg-dist=00;90:*.dpkg-new=00;90:*.dpkg-old=00;90:*.dpkg-tmp=00;90:*.old=00;90:*.orig=00;90:*.part=00;90:*.rej=00;90:*.rpmnew=00;90:*.rpmorig=00;90:*.rpmsave=00;90:*.swp=00;90:*.tmp=00;90:*.ucf-dist=00;90:*.ucf-new=00;90:*.ucf-old=00;90:
VTE_VERSION=7603
GIO_EXTRA_MODULES=/nix/store/3zi7zn2bbz3jpx8ds4nharz67j6ajp9k-xfconf-4.18.3/lib/gio/modules:/nix/store/xgc117gcsq0y0cc4vw0szk02wx0dlbh3-dconf-0.40.0-lib/lib/gio/modules:/nix/store/3zi7zn2bbz3jpx8ds4nharz67j6ajp9k-xfconf-4.18.3/lib/gio/modules:/nix/store/xgc117gcsq0y0cc4vw0szk02wx0dlbh3-dconf-0.40.0-lib/lib/gio/modules:/nix/store/3zi7zn2bbz3jpx8ds4nharz67j6ajp9k-xfconf-4.18.3/lib/gio/modules:/nix/store/xgc117gcsq0y0cc4vw0szk02wx0dlbh3-dconf-0.40.0-lib/lib/gio/modules:/nix/store/3zi7zn2bbz3jpx8ds4nharz67j6ajp9k-xfconf-4.18.3/lib/gio/modules:/nix/store/xgc117gcsq0y0cc4vw0szk02wx0dlbh3-dconf-0.40.0-lib/lib/gio/modules:/nix/store/xgc117gcsq0y0cc4vw0szk02wx0dlbh3-dconf-0.40.0-lib/lib/gio/modules:/nix/store/xgc117gcsq0y0cc4vw0szk02wx0dlbh3-dconf-0.40.0-lib/lib/gio/modules:/nix/store/3zi7zn2bbz3jpx8ds4nharz67j6ajp9k-xfconf-4.18.3/lib/gio/modules:/nix/store/xgc117gcsq0y0cc4vw0szk02wx0dlbh3-dconf-0.40.0-lib/lib/gio/modules:/nix/store/3zi7zn2bbz3jpx8ds4nharz67j6ajp9k-xfconf-4.18.3/lib/gio/modules:/nix/store/xgc117gcsq0y0cc4vw0szk02wx0dlbh3-dconf-0.40.0-lib/lib/gio/modules:/nix/store/3zi7zn2bbz3jpx8ds4nharz67j6ajp9k-xfconf-4.18.3/lib/gio/modules:/nix/store/xgc117gcsq0y0cc4vw0szk02wx0dlbh3-dconf-0.40.0-lib/lib/gio/modules:/nix/store/3zi7zn2bbz3jpx8ds4nharz67j6ajp9k-xfconf-4.18.3/lib/gio/modules:/nix/store/xgc117gcsq0y0cc4vw0szk02wx0dlbh3-dconf-0.40.0-lib/lib/gio/modules
FLAG=pwn.college{E7C3ZA0jdeOrjeaHxEZ8-lEa44_.dhTN1QDLzETN0czW}
LESSCLOSE=/usr/bin/lesspipe %s %s
TERM=xterm-256color
LESSOPEN=| /usr/bin/lesspipe %s
DISPLAY=:0.0
SHLVL=2
LC_CTYPE=C.UTF-8
XDG_DATA_DIRS=/nix/store/14x11ifwhnw8fhjdxs94q7hivhdqslgx-xfce4-terminal-1.1.3/share:/nix/store/szyhy2fbbm1318qrkl6p4j5ibx6xykl4-gsettings-desktop-schemas-46.0/share/gsettings-schemas/gsettings-desktop-schemas-46.0:/nix/store/mlzl5gqfnbvrpy44zd2d5zdv1r04x977-gtk+3-3.24.43/share/gsettings-schemas/gtk+3-3.24.43:/nix/store/4mnz50gh5j2sss4pm74wvzqzg1w46ax1-xfce4-settings-4.18.4/share:/nix/store/szyhy2fbbm1318qrkl6p4j5ibx6xykl4-gsettings-desktop-schemas-46.0/share/gsettings-schemas/gsettings-desktop-schemas-46.0:/nix/store/mlzl5gqfnbvrpy44zd2d5zdv1r04x977-gtk+3-3.24.43/share/gsettings-schemas/gtk+3-3.24.43:/nix/store/ykksrxmcqdk67ca0821frjdry2c6pfsq-exo-4.18.0/share:/nix/store/szyhy2fbbm1318qrkl6p4j5ibx6xykl4-gsettings-desktop-schemas-46.0/share/gsettings-schemas/gsettings-desktop-schemas-46.0:/nix/store/mlzl5gqfnbvrpy44zd2d5zdv1r04x977-gtk+3-3.24.43/share/gsettings-schemas/gtk+3-3.24.43:/nix/store/xpgf309sv9w5majf26zg50fpd9vqk1x3-xfce4-panel-4.18.6/share:/nix/store/szyhy2fbbm1318qrkl6p4j5ibx6xykl4-gsettings-desktop-schemas-46.0/share/gsettings-schemas/gsettings-desktop-schemas-46.0:/nix/store/mlzl5gqfnbvrpy44zd2d5zdv1r04x977-gtk+3-3.24.43/share/gsettings-schemas/gtk+3-3.24.43:/nix/store/jnz1wdn463qilzhc8nj1kwccshk65pc9-xfce4-session-4.18.3/share:/nix/store/szyhy2fbbm1318qrkl6p4j5ibx6xykl4-gsettings-desktop-schemas-46.0/share/gsettings-schemas/gsettings-desktop-schemas-46.0:/nix/store/mlzl5gqfnbvrpy44zd2d5zdv1r04x977-gtk+3-3.24.43/share/gsettings-schemas/gtk+3-3.24.43:/run/dojo/share:/usr/local/share:/usr/share
PATH=/run/challenge/bin:/run/workspace/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
DBUS_SESSION_BUS_ADDRESS=unix:path=/tmp/dbus-nH79jM6mzg,guid=ccfb0c030f6c0a61d7baa9016707cfd6
_=/run/workspace/bin/env

```
