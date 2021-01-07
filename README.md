# helper-scripts

A collection of small, simple CLI utilities that I use regularly for 
various things.

## ccolor

This is a python script that can convert between RGB, HEX, HSL, and CMYK. By
default it will convert to all the supported types, but you can specify which
one you want by using the `--to=FMT` flag.

You could probably use this to automate some aspects of web development since
its output is HTML/CSS compliant. Eventually I'll expand on this aspect by
enabling it to read the color from `stdin`

## lsusb-follow

Another python script which runs `lsusb` continuously and outputs without
filling up your console. This is a little easier to digest than watching
dmesg, and it doesn't require root. `lsusb` is included in the `moreutils`
package on most distros.

## screenshot

Exactly what it says it is. This simply takes a screenshot of the entire
X screen and saves it to `~/Pictures/screenshots`

## tcomp

This on is more niche. On the rounded-corners version of picom, sometimes on
launch or settings reload, either the blur or the rounded corners won't appear.
This simply touches the config file, causing the program to reset.
