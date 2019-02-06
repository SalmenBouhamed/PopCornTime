### 1. Downloading

32 bits version

``` bash
$ wget https://get.popcorntime.sh/build/Popcorn-Time-0.3.10-Linux-32.tar.xz -O popcorntime.tar.xz
```

64 bits version

``` bash
$ wget https://get.popcorntime.sh/build/Popcorn-Time-0.3.10-Linux-64.tar.xz -O popcorntime.tar.xz
```

### 2. Unpacking

``` bash
$ sudo mkdir /opt/popcorntime; sudo tar Jxf popcorntime.tar.xz -C /opt/popcorntime
```

### 3. Creating a shortcut

``` bash
$ sudo ln -sf /opt/popcorntime/Popcorn-Time /usr/bin/Popcorn-Time
```

### 4. Creating the application launcher

``` bash
$ sudo nano /usr/share/applications/popcorntime.desktop
```

``` text
[Desktop Entry]
Version=1.0
Type=Application
Terminal=false
Name=PopCorn
Exec=/opt/popcorntime/Popcorn-Time
Icon=/opt/popcorntime/src/app/images/icon.png
Categories=Application;
```

### 5. Delete the downloaded file

``` bash
$ rm popcorntime.tar.xz
```

### Uninstall

``` bash
$ sudo rm -Rf /opt/popcorntime
$ sudo rm /usr/bin/Popcorn-Time
$ sudo rm /usr/share/applications/popcorntime.desktop
```
