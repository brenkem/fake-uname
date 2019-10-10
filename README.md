# fake uname
Tool to fake the output of the 'uname' command in chroot and other enviroments
to adjust the used kernel version in uname calling Makefiles.


For example to prepare the system to use fake-uname just rehash uname
from /bin/uname to /tmp/uname with the following command:
    hash -p /tmp/uname uname

## currently supported options
    -r, --kernel-release     Release‐Nummer des Kernels ausgeben
    -m, --machine            print the machine hardware name

## missing options
    -a, --all                alle Informationen ausgeben, in der folgenden
                               Reihenfolge (außer -p und -i, wenn nicht bekannt):
    -s, --kernel-name        Namen des Kernels ausgeben
    -n, --nodename           Netzwerknamen der Maschine ausgeben
    -v, --kernel-version     print the kernel version
    -p, --processor          print the processor type (non-portable)
    -i, --hardware-platform  print the hardware platform (non-portable)
    -o, --operating-system   print the operating system
        --help     diese Hilfe anzeigen und beenden
        --version  Versionsinformation anzeigen und beenden

Please feel free to implement missing options and perform a pull request.
