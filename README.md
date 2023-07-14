# Threshold-Alpha-2---Gimp-Plugin
A better version of Gimp's threshold alpha filter that mimicks curves on alpha and can be called from GEGL Graphs. This is meant to be a component for GEGL Plugins not really a stand alone use. As a normie would be better suited using curves on alpha.



![image](https://github.com/LinuxBeaver/Threshold-Alpha-2---Gimp-Plugin/assets/78667207/6d731c1b-2237-40fb-b709-a8c1aa8609e8)
For more info on the seperate Glossy Balloon text styling plugin go here.
https://github.com/LinuxBeaver/GEGL-glossy-balloon-text-styling

## OS specific location to put GEGL Filter binaries 

Windows
 C:\\Users\<YOUR NAME>\AppData\Local\gegl-0.4\plug-ins
 
 Linux 
 /home/(USERNAME)/.local/share/gegl-0.4/plug-ins
 
 Linux (Flatpak)
 /home/(USERNAME)/.var/app/org.gimp.GIMP/data/gegl-0.4/plug-ins

 ### Linux

To compile and install you will need the GEGL header files (`libgegl-dev` on
Debian based distributions or `gegl` on Arch Linux) and meson (`meson` on
most distributions).

```bash
meson setup --buildtype=release build
ninja -C build

```

If you have an older version of gegl you may need to copy to `~/.local/share/gegl-0.3/plug-ins`
instead (on Ubuntu 18.04 for example).



### Windows

The easiest way to compile this project on Windows is by using msys2.  Download
and install it from here: https://www.msys2.org/

Open a msys2 terminal with `C:\msys64\mingw64.exe`.  Run the following to
install required build dependencies:

```bash
pacman --noconfirm -S base-devel mingw-w64-x86_64-toolchain mingw-w64-x86_64-meson mingw-w64-x86_64-gegl
```

Then build the same way you would on Linux:

```bash
meson setup --buildtype=release build
ninja -C build
```


## Previews of this based Gimp Plugin and WHAT IT IS SUPPOSE TO DO PRACTICALLY

![image](https://github.com/LinuxBeaver/Threshold-Alpha-2---Gimp-Plugin/assets/78667207/c64b3f4b-4464-4bfa-86a9-a1c9c6854bda)


![image](https://github.com/LinuxBeaver/Threshold-Alpha-2---Gimp-Plugin/assets/78667207/98de8b71-0b28-4b75-bd65-46002c27eedf)

![image](https://github.com/LinuxBeaver/Threshold-Alpha-2---Gimp-Plugin/assets/78667207/821ee12a-16f4-4ad5-8781-237791f9e5f4)

