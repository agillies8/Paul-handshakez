# Hollywood Handshake Index

Every Paul Hollywood handshake on *The Great British Bake Off*, series 1 to series 17 week 3: 65 handshakes across 157 episodes, with the baker, bake, challenge, week, and what happened to them afterwards.

## Run it

It is a static site with no build step. The page fetches its data, so serve the folder rather than opening the file directly:

```sh
python3 -m http.server 8000
# then open http://localhost:8000
```

## Layout

- `index.html` is the whole page (styles and script inline).
- `data/handshakes.json` is what the page loads: `meta`, `handshakes`, `episodes` and `series`.
- `data/handshakes.csv` holds one row per handshake.
- `data/episodes.csv` holds one row per episode, with its handshake count.

Timestamps and exact clip URLs are blank because they could not be verified; each handshake links to a YouTube search instead. Sources are listed in `meta.sources` in the JSON.
