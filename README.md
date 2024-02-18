# Calendar thing

This is a calendar thing that i use to keep track of stuff, like a diary. It's a single HTML file witha bunch of JS inside. It reads data from two files, one for points in time and one for durations.

To edit colors, file URL's, etc - just change the HTML file.

## File formats

`timeline.dat` is for points in time. Follows this format:

```
yyyy-mm-dd:some text
yyyy-mm-dd:some other thing {https://optional link/}

 blank lines allowed, i feel it helps separating months into chunks.
   comments start with one or more spaces like this
yyyy-mm-dd:more stuff happened
```

`data.txt` for timespans. CSV like:

```
yyyy-mm-dd;yyyy-mm-dd;some text
;yyyy-mm-dd;some thing with only an end date
yyyy-mm-dd;;some thing with only a start date

blank lines allowed. all lines _without_ semicolons in them are comments.
yyyy-mm-dd;yyyy-mm-dd;some text with both a start and end date
```

## Screeny shot

![demo](https://raw.githubusercontent.com/free-ghz/calendar/main/demo.png "demo")
