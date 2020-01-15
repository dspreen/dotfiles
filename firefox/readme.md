I enjoy reading web articles in a distraction-free reader mode. Firefox—my browser of choice—offers such a mode, but it's quite ugly which is a distraction in itself. I liked the way safari did it, so I took some inspiration to put together my own style sheet. Here's what I came up with.

If you want to use this, you need to create a "chrome" directory in your firefox profile and place it inside. (Instructions for some of this adapted from https://github.com/bit101/dotfiles/tree/master/firefox).

1. In Firefox, open `about:profiles`.
2. Open the directory called `Root Directory` in a terminal. 
3. Either `cd chrome` or `mkdir chrome && cd chrome`.
4. Place userContent.css from this repository inside that folder.
5. If you are using an older version of Firefox, just restart the browser and you're good to go.

For users of Firefox 69 and above, the following additional step is necessary:

6. In Firefox, open `about:config`.
7. Search for the configuration key `toolkit.legacyUserProfileCustomizations.stylesheets`.
8. Make sure the toggle is set to `true`.
9. Restart Firefox.

Note: I don't care for sepia, so I am using it for a third style that resembles the first iteration of macOS's dark mode: dark context but light content.

The result should look like this:

![Example Article in Light Mode](screenshot-light.png?raw=true "Example Article in Light Mode")

![Example Article in Dark Mode](screenshot-dark.png?raw=true "Example Article in Dark Mode")

![Example Article in Sepia Mode](screenshot-sepia.png?raw=true "Example Article in 'Sepia' Mode")
