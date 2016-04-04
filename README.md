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

## Exact Steps

1. Clone this git repo to your machine
`git clone https://github.com/bradfa/mr-oe-bonedev.git`
2. List the path to the `.mrconfig` file within the `mr-oe-bonedev` git
repository in your `~/.mrtrust` file.  If you cloned the `mr-oe-bonedev` git
repository into your `~/git/` directory, you'd use a line like
`~/git/mr-oe-bonedev/.mrconfig` to do this.
3. Change into the `mr-oe-bonedev` directory and issue the `mr checkout`
command.  This will proceed to checkout all the needed git repos and setup some
basic remote repositories for you (which currently point to my own github
repos).
4. Do some work and read the `mr help` output.
