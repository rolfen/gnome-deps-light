## What?

The gnome-deps-light virtual package provides stubs which enable you to remove bloaty gnome dependencies.

## Why?

There are a few mandatory packages that get installed with gnome, but which I never use. I would like to remove them to free some space. However gnome would not let me.  
So I created this "virtual package" which "provides" these dependencies, thereby allowing me to delete the said packages.

## A package, where?

This is the source for building a `.deb` package.
It relies on the tool `equivs` for quickly building virtual packages. 

## Building

Install `equivs` then have a look at `/usr/share/doc/equivs/README.Debian`.
