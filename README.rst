UUID
====

This library is copied from the
`util-linux <http://en.wikipedia.org/wiki/Util-linux>`_ package.

It was written by Theodore Ts'o and it is BSD licensed.

This git repository adds a CMake buildsystem and an spkg-install file. It
leaves the original autotools Makefile.am/in files intact, so that once can
debug the CMake build system if it is doing something different (link options,
etc.).

Motivation
----------

The motivation for this repository is so that one can easily install just the uuid library, needed by some other packages (like `zeromq <http://www.zeromq.org/>`_), without the need to install the whole ``util-linux`` package.

Install
-------

Just like any other cmake based project::

    cmake -DCMAKE_INSTALL_PREFIX="somewhere" .
    make
    make install

Look into the ``spkg-install`` file for an example.
