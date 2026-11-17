# Vinyl Records

An interactive record player for iPad (12.9″, landscape or portrait), phones and desktop browsers.
Pick a record, take it out of its sleeve, and turn the dial to blend the unprocessed
recording into the version processed for the venue.

## What's in this folder

| File | What it is |
|---|---|
| `index.html` | The page itself (about 60 KB). |
| `assets/img/` | The record prints and sleeve prints. |
| `assets/audio/` | The recordings: a dry and a processed take for each record. |
| `.nojekyll` | Tells GitHub Pages to serve the files as they are. Optional. |

The page loads its pictures and sound from `assets/`, so upload the whole folder, keeping `assets` next to `index.html`.

## Put it online with GitHub Pages

1. On github.com, create a new repository (for example `vinyl-records`). Free accounts need it public for Pages.
2. Click **Add file → Upload files**, drag in everything from this folder (the `assets` folder included), and click **Commit changes**.
3. Go to **Settings → Pages**. Under **Build and deployment**, set **Source** to *Deploy from a branch*, choose `main` and `/ (root)`, then **Save**.
4. After a minute or two the page shows your link, like `https://your-name.github.io/vinyl-records/`. Open it on the iPad.

Tip: in Safari on the iPad, tap **Share → Add to Home Screen** to open it full screen like an app.

## The records

| # | Genre | Venue | Colour | Recordings |
|---|---|---|---|---|
| 1 | Rock | Arena | Blue | rock-dry / rock-arena |
| 2 | Pop | Theatre | Pink | pop-dry / pop-theatre |
| 3 | Soul | Arena | Orange | soul-dry / soul-arena |
| 4 | Folk | Theatre | Green | folk-dry / folk-theatre |

## Using it

- **Switch records:** tap the arrows, use the ← → keys, or swipe. Records move in the direction you go: the next one comes in from the right.
- **Listen:** tap the record to take it out of its sleeve. Tap it again to put it back.
- **Process the sound:** turn the dial. Every record starts at 10% processed.
- **Credits:** tap Credits in the bottom-right corner while choosing a record; Back returns.

## Swapping in new records

Replace the files in `assets/` with new ones of the same name, or add new files and point to them
in the `RECORDS` list near the top of the script in `index.html`
(`photo` = record print, `card` = sleeve print, `track` = which pair of recordings).

## Good to know

- The page needs an internet connection: the 3D library (three.js) and the typeface load from the web.
- Sound starts after a tap, as browsers require. It plays even with the iPad in silent mode on iPadOS 17 and later.
- Opening `index.html` straight from your computer's folders won't play sound; it needs to be served, as GitHub Pages does.
- The typeface is a stand-in (Hanken Grotesk) until an Apfel Grotezk font file is added.
