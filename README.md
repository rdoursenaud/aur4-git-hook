Git Hook for Arch Linux AUR4 packaging
======================================

The
[AUR4 documentation](https://wiki.archlinux.org/index.php/Arch_User_Repository#AUR_4)
insists on the fact that ```.SRCINFO``` must be generated and added at each commit.

Since I'm prone to forgetting such things, I cooked a very simple git hook
that does it for me just before committing.

Just make sure that
[pkgbuild-instrospection](https://www.archlinux.org/packages/?name=pkgbuild-introspection)
is installed.

Usage
-----

Just place the ```pre-commit``` file in the ```.git/hooks/``` directory in
your AUR4 git clone and make sure it's executable.
