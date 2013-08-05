diagrams-sources
================

This repository contains a `sources.txt` file in the format expected by
[cabal-meta](https://github.com/yesodweb/cabal-meta).  This allows you to build
and develop the most recent HEAD versions of the diagrams packages.

Usage
-----

```
git clone https://github.com/diagrams/diagrams-sources.git
cd diagrams-sources
cabal-meta install
```

If all goes well, the HEAD versions of all the diagrams packages will now be in
the `vendor/` directory, and be installed to your local cabal package database.

Notes
-----

The following https://github.com/diagrams/ repositories aren't included:

* Due to no `*.cabal` file:
    - `diagrams/diagrams-test`
    - `diagrams/diagrams-doc`
* Due to compatibility issues (the hackage version works fine):
    - `diagrams/active`
