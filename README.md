# archlinux
A repository for system configuration files. x64 Arch Linux : Acer C720 32.0GB internal SSD.

Notes about package list generation:

* 'packages_native.txt' was generated with the command: 'pacman -Qqetn > packages_native.txt'

... This generates a text file that contains package names for packages that were explicitly installed 
by 
the user, not dependent on any other package (so not installed as a dependency), and are native to the pacman 
package database on your system (e.g. emacs) as opposed to a user-level community package (e.g. google-chrome web browser from the aur). Note that some of these packages may require other system packages to be 
installed (e.g. base-devel and btrfs-progs).

* 'packages_community.txt' was generated with the command: 'pacman -Qqm > packages_community.txt'

... This generates a text file that contains package names for community packages that were installed by 
the user (e.g. google-chrome web browser from the aur).

* INSTALLATION : To expedite the process of package installation from the native package list, you can use the command "pacman -S `cat packages_native.txt`"
