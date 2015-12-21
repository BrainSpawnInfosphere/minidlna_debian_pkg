# MiniDLNA Package

Creating a minidlna debian package for the RPi since the current version for raspbian is very old.

http://stackoverflow.com/questions/15483725/debian-package-creation-how-to-install-configuration-files

http://askubuntu.com/questions/170348/how-to-make-my-own-local-repository

# Structure

    template (directory)
    template/debian (directory)
    template/debian/control
    template/debian/changelog
    template/debian/displace
    template/debian/rules
    template/debian/postinst
    template/debian/install
    template/debian/docs
    template/debian/compat
    template/README
    template/BUILD
    template/files (directory)

where `template/files` is a directory like `etc` or `usr`.

## Test Package

    $ mkdir /tmp/t
    $ dpkg-deb -x foo.deb /tmp/t
    $ ls /tmp/t
