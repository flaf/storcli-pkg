# Debian Package Storcli (for amd64 architecture)

`stocli` is a binary to manage LSI MegaRAID controllers.

**Remark:** here it's the 64-bit version of `storcli`.

To build the package on **Debian Jessie** (but the package
could be used in another distributions), you have to clone
the Git repository, make a `cd` in your local Git repository
and launch these commands:

```sh
sudo apt-get install --no-install-recommends build-essential devscripts fakeroot debhelper lintian
debuild -b -us -uc --lintian-opts --pedantic -i -I && echo 'Building is OK!'
ls -l ../storcli*.deb
```

# How to download the `storcli` binary

As far as I know, there is no source code for the binary
`storcli` and you can download the latest version of this
file in
[this page](https://www.broadcom.com/support/download-search)
(search the keyword `storcli`). Attention, normally the
binary is called `storcli64`.


