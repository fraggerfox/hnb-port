hnb-port
========

FreeBSD [Ports][3] script for Hierarchical Notebook (hnb).

You can find Hierarchical Notebook (hnb) [here][1] a fixed version of hnb that
runs on amd64 can be found [here][4].

NOTE: This is not a new package, but is a fixed version of the package that can
run in both i386 and amd64

Installation
------------

Copy `editors/hnb` folder to `/usr/ports` directory.

NOTE: If your ports directory is different from above, copy to the respective
place.

Usage
-----

Once you have copied the folder, install it as you would do for any port.

`$ cd /usr/ports/editors/hnb`<br>
`$ make install clean`

For a list of dependencies for the build check [here][2]

Credits
-------

* Hierarchical Notebook (hnb) was originally written by `Øyvind Kolås`
* The original ports script was written by `pat@databits.net`
* Thanks to `amdmi3@` for reviewing and suggesting fixes / changes to the ports
  script.
* Thanks to `@ppaeps` for helping me debug the amd64 crashes.

License
-------

BSD 2-clause. See LICENSE.

[1]: http://hnb.sourceforge.net/
[2]: http://hnb.sourceforge.net/Documentation/
[3]: http://freshports.org/editors/hnb
[4]: https://github.com/fraggerfox/hnb
