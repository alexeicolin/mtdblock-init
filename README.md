Init script for creating `/dev/mtdblock` device node for each existing
`/dev/mtd` node.

On Javelin S4, the udev in Debian Wheezy does not create the `mtdblock` device
nodes but only the `mtd` nodes, despite the kernel having `mtdblock` built in.
