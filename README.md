# tilde-town

Source for my [tilde.town](https://tilde.town) personal page — **~chumthewaters**.

- **Lives at:** https://tilde.town/~chumthewaters/
- **Theme:** "chum the waters" 🦈 — a dense ASCII shark that swims the deep, turns to face where it's going, and chases your cursor (click to toss it chum).
- **Stack:** vanilla HTML + CSS + a sprinkle of plain JS (no frameworks, no build step) — tilde.town pages are hand-made and lightweight.
- **Files:** `index.html` (markup + shark sim) + `style.css` + `shark-frames.js` (the ASCII frame data). That's the whole reef.

## Deploy
tilde.town serves `~/public_html/index.html`. Push the page over SSH (requires a tilde.town
account + SSH access as `chumthewaters`):

```sh
# from this repo
scp index.html style.css shark-frames.js chumthewaters@tilde.town:~/public_html/
# or keep it in sync:
rsync -av --exclude '.git' ./ chumthewaters@tilde.town:~/public_html/
```

> No tilde.town account yet? Apply at https://tilde.town/ (it's an invite/application pubnix).

## Credits
The swimming shark's ASCII frames are adapted from **"Ascii Shark"** by **Kitty (`meowinglion`)** —
[Wallpaper Engine Workshop #3606705311](https://steamcommunity.com/sharedfiles/filedetails/?id=3606705311).
The frame data is cropped to a subset (12 headings × 16 swim frames) and re-serialized for the web;
the swim/steer/cursor-chase behaviour is a fresh vanilla-JS reimplementation.
