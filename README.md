# tilde-town

Source for my [tilde.town](https://tilde.town) personal page — **~chumthewaters**.

- **Lives at:** https://tilde.town/~chumthewaters/
- **Theme:** "chum the waters" 🦈 — a hand-made ASCII shark that swims the deep, turns to face where it's going, and chases your cursor (click to toss it chum).
- **Stack:** vanilla HTML + CSS + a sprinkle of plain JS (no frameworks, no build step) — tilde.town pages are hand-made and lightweight.
- **Files:** `index.html` (markup + the shark sim) + `style.css`. That's the whole reef.

## Deploy
tilde.town serves `~/public_html/index.html`. Push the page over SSH (requires a tilde.town
account + SSH access as `chumthewaters`):

```sh
# from this repo
scp index.html style.css chumthewaters@tilde.town:~/public_html/
# or keep it in sync:
rsync -av --exclude '.git' ./ chumthewaters@tilde.town:~/public_html/
```

> No tilde.town account yet? Apply at https://tilde.town/ (it's an invite/application pubnix).
