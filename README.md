# chumthewaters — ASCII shark

A dense **ASCII shark** that swims the deep, turns to face where it's heading, and chases your
cursor — click to toss it chum. The "chum the waters" mascot, as a tiny self-contained web animation.

- **Stack:** vanilla HTML + CSS + a little plain JS — no frameworks, no build step.
- **Files:** `index.html` (markup + shark sim), `style.css`, and `shark-frames.js` (the ASCII frame data).

## Use it

Three static files. Open `index.html` directly, or drop them on any static host:

```sh
scp index.html style.css shark-frames.js user@host:~/public_html/
```

## Credits

The swimming shark's ASCII frames are adapted from **"Ascii Shark"** by **Kitty (`meowinglion`)** —
[Wallpaper Engine Workshop #3606705311](https://steamcommunity.com/sharedfiles/filedetails/?id=3606705311).
The frame data is cropped to a subset (12 headings x 16 swim frames) and re-serialized for the web; the
swim / steer / cursor-chase behaviour is a fresh vanilla-JS reimplementation.
