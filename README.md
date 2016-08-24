myrepos Development Environment for OE
======================================

This is mostly an example for others, but is useful for me, for doing
development of OE recipes and for testing Linux and U-Boot code changes.

This repository uses the myrepos tool to coordinate subdirectory git
repositories as needed.  This, in theory, will allow easier use by others as
they can simply get up and running with the same sources as me very quickly.

## Prereqs

You will need the [myrepos](https://myrepos.branchable.com/) tool installed from
your package manager along with all of the normal prerequisites listed in the
[Yocto Project
documentation](https://www.yoctoproject.org/docs/latest/mega-manual/mega-manual.html#packages).

## Exact Steps for Getting Set Up

1. Clone this git repo to your machine:
`git clone https://github.com/bradfa/mr-oe-bonedev.git`
2. Change into the cloned repo: `cd mr-oe-bonedev`
3. List the path to the `.mrconfig` file within the `mr-oe-bonedev` git
repository in your `~/.mrtrust` file so that myrepos will trust this repo to
execute: `echo $(pwd)/.mrconfig >> ~/.mrtrust`
4. Checkout all the needed git repos and setup some basic remote repositories
for you: `mr checkout`
5. Do some work and read the `mr help` output.

## Exact Steps for Building a Linux Distribution

1. 
