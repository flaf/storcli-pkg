# Debian Package Storcli

`stocli` is a binary to manage LSI MegaRAID controllers.

To build the package on **Debian Jessie**, you have to clone
the Git repository, make a `cd` in your local Git repository
and launch these commands:

```sh
apt-get install devscripts
debuild -b -us -uc --lintian-opts --pedantic -i -I && echo 'Building is OK!'
ls -l ../stocli*.deb
```


