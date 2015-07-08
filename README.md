brick
-----

`brick` is a terminal user interface programming
library written in Haskell, in the style of
[gloss](http://hackage.haskell.org/package/gloss). This means you write
a function that describes how your user interface should look, but the
library takes care of a lot of the book-keeping that so commonly goes
into writing such programs.

The API exposed by `brick` is purely functional. Unlike most GUI
toolkits which require you to write a long and tedious sequence of
"create a widget, now bind an event handler", `brick` just requires you
to describe your interface -- even the bits that are stateful -- using
a set of declarative combinators and it does the rest. All you have to
do is provide functions to transform your own application state when
input (or other kinds of) events arrive.

Under the hood, this library uses [vty](http://hackage.haskell.org/package/vty).

This library deprecates [vty-ui](https://github.com/jtdaugherty/vty-ui).
Some day `brick`, too, will have a [70-page
manual](http://jtdaugherty.github.io/vty-ui/manuals/vty-ui-users-manual-1.9.pdf).

Getting Started
---------------

The best way to get started is to build, run, and read the source for
the various demonstration programs in the `programs/` directory. This
will help you get to know the library and what it can do. There is also
extensive Haddock documentation.

```
$ cabal sandbox init
$ cabal install -j
$ .cabal-sandbox/bin/brick-???-demo
```
