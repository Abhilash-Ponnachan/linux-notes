# Linux Commands 
----------------

## The Shell
------------
The _shell_ is a program that takes keyboard inputs and sends them to the OS to execute. Almost all _Linux_ distros supply a _shell_ from the _GNU_ project called `bash` (_bourne again shell_ after the author Steve Bourne of the original _UNIX_ shell _sh_).  

### Terminal Emualators
When using a GUI we woudl use a _terminal emulator_ program to interact with the shell.  
_KDE_ has a program called `konsole`  
_GNOME_ has one called `gnome-terminal`  
Though all of these would generally show up as `Terminal` in your menu.

**Using the Mouse**  
The _terminal_ is all about using the _keyboard_. One handy trick to copy & paste text is to use the mouse to _highlight_ some text - this will copy it into a buffer, and we can paste it where the cursor is at using the _middle mouse buton_. This is implemented by the _X windows_ system that underpins the _Linux GUI_. Note that `Ctrl + C` & `Ctrl + V` does not work in _Linux_ terminals.

## Trying Some Commands
-----------------------
Let us take it for a spin and try out some commands just to whet our apptetite -
```shell
$ date
Wed 18 Sep 10:41:25 BST 2019

$ cal
   September 2019     
Su Mo Tu We Th Fr Sa  
 1  2  3  4  5  6  7  
 8  9 10 11 12 13 14  
15 16 17 18 19 20 21  
22 23 24 25 26 27 28  
29 30                 
```
To see our storage devices information we could use `df`
```shell
$ df
Filesystem     1K-blocks     Used Available Use% Mounted on
udev             4001276        0   4001276   0% /dev
tmpfs             806304     9736    796568   2% /run
/dev/sda7      102586680 22617272  74735184  24% /
tmpfs            4031508    93224   3938284   3% /dev/shm
tmpfs               5120        4      5116   1% /run/lock
tmpfs            4031508        0   4031508   0% /sys/fs/cgroup
/dev/sda1         507904    62304    445600  13% /boot/efi
tmpfs             806304       72    806232   1% /run/user/1000
```
Likewise to see our free memory we can do -
```shell
$ free
              total        used        free      shared  buff/cache   available
Mem:        8063016     1633848     3984024      618584     2445144     5420076
Swap:       8283132           0     8283132
```

## Navigating the File System
-----------------------------
Let 