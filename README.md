# mac-vol
A simple script for changing the volume on a Mac, for when your keyboard
doesn't have volume controls.

## Why?
I wrote this script because if your keyboard doesn't have volume keys it seems
to be quite difficult to change the volume on your Mac. My Google-fu just brought
up lots of links to 3rd party scripting utilities which can then be connected to
keyboard shortcuts. Since I almost always have a terminal open for other purposes
writing a script that can be put into your path seemed like the simplest and most
elegant solution.

## How?
The script is relatively easy to invoke. There are 7 "levels" of volume.

```bash
$ vol get
> Volume is 3
$ vol up
> Volume is 4
$ vol down
> Volume is 3
$ vol 0
> Volume changed from 3 to 0
```
