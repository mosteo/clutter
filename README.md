# clutter
Command-Line Utilities for Linux

A collection of perhaps-useful scripts I've needed during my researcher life:

### fit2mp4 <file> <size> \[--fast] \[other ffmpeg options]
Size understands postfixes (whatever numfmt accepts).
Takes any video and fits it into a given size mp4, by dichotomic quality adjusting.
If quality alone does not give good results, adjusting resolution will surely help.
