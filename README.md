**This *(outdated repo)* is an educative/experimental example of how to use `equivs` to create "stubs packages" in debian / ubuntu**

## What?

The gnome-deps-light virtual package provides stubs which enable you to remove bloaty gnome dependencies.

In this context, a "stub" is an empty package which could replace a real package.

This hack can break your system, test throughly and use at your own risk.

## Why?

There are a few mandatory packages that get installed with gnome, but which I never use. I would like to remove them to free some space. However the packaging manager would not let me because they are listed as dependencies of gnome. 

They are very simple yet relatively big packages which I don't use.

So I created this "fake", empty package which "provides" these dependencies and also "conflicts" with them thereby triggering the package manager to uninstall them.

## A package, where?

This is the source for building a `.deb` package.
It relies on the tool `equivs` for quickly building virtual packages. 

## Building, how?

Install `equivs` then have a look at `/usr/share/doc/equivs/README.Debian`.
