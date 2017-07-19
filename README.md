# clutter
Command-Line Utilities for Linux

A collection of perhaps-useful scripts I've needed during my researcher life. They may depend on other debian packages that you'll probably discover by trial-and-error, since there's no checking for pre-requisites being installed.

They should work when given proper inputs, but there's no special effort to screen parameters.

`any2mp3 [-c|-v] <file>`
* Transcodes anything that ffmpeg understands into a constant/variable bitrate mp3.

`any2mp4 <file>`
* Transcodes anything that ffmpeg understands into an mp4.

`avtrim <src> <start time> <end time> <dest>`
* Extracts (without transcoding) a video clip.
* Understands hh:mm:ss format for start/end times.

`baobab-nox [path]`
* Reports graphically and textually the size of files/folders in the given/current path.

`fit2mp4 <file> <size> [--fast] [other ffmpeg options]`
* Size understands postfixes (whatever numfmt accepts).
* Takes any video and fits it into a given size mp4, by dichotomic quality adjusting.
* If quality alone does not give good results, adjusting resolution will surely help.
* Output is in original_name.quality.mp4

`run-when-idle <seconds> <command>`
* Forever starts/stops (sigterm, and sigkill after 5s if TERM failed) a command when the user (as determined by the X server) is idle for the given seconds.

`seconds2date <seconds>`
* Formats a number into a dd:hh:mm:ss string.

`ttic / ttoc [-h]`
* ttoc reports (optionally in human-friendly format) seconds elapsed since the last ttic. Useful when `time` is not enough for reasons.
