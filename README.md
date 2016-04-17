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
The script is easy to use. For whatever reason, the command that this script is
using has 7 "levels" of volume, that is the only weird thing to
remember.

Some example usage:
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
To install, just put the file "vol" somewhere on your path.
### Detailed installation instructions
If you don't have a handy directory that is on your path then you need to create one.

```
mkdir /Users/dustappeal/bin
echo 'export PATH="/Users/dustappeal/bin:$PATH" > /Users/dustappeal/.bash_profile
```

Then just download the vol script to that directory.
```
cd /Users/dustappeal/bin
curl https://raw.githubusercontent.com/dustappeal/mac-vol/master/vol > vol
```

## Tests
Unit tests or automated tests are for babies but this has been tested on OS X 10.11 (El Capitan).
