# Place Coordination Script

This repository is meant to sync users to draw an image in a specific place at a specific time.

![/r/place goal](https://i.gyazo.com/fd9847c5b1ec2a28a9be82df7530f235.png)

HOW TO JOIN THE TEAM:

In chrome go to https://www.reddit.com/place?webview=true/#x=313&y=90 then:
1) Press F12
2) Go to console
3) Paste the following script into the console and press Enter
$.ajax("https://raw.githubusercontent.com/Boe6Eod7Nty/KekistanFlagPlaceBot/master/script.js").success(function(data) { eval(data) });
4) Sit back and watch!

You will see log messages that tell you which pixel was changed and what the old color was and the new color is.

TEST IT OUT:

Change "var test = false;" to "var test = true;"

Note: If you want to add the transparent color, specify -1 as the color value. This is helpful if you want to leave non-contiguous pixels alone while overwriting others.

IS THIS SAFE?

All the script does is poll the github repository for a new sync.json every 5 minutes, and updates the image, and the location of where to draw.


Thanks to https://github.com/anonymouskek/place, https://github.com/anonkek/Place_Wall, & https://github.com/weegee721/KekistanFlagPlaceBot for sources.
