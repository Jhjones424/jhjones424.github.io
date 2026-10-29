# jhjones424.github.io

The root of the GitHub Pages host. It exists for one file: `.well-known/apple-app-site-association`, which tells iOS
that FlopShot's add-a-friend links (`https://jhjones424.github.io/flopshot-legal/add?u=<handle>`) open the FlopShot app.
Apple only reads that file at the root of a host, so it can't live in the `flopshot-legal` repo.

- `.nojekyll` makes GitHub Pages publish the `.well-known` folder (Jekyll skips folders starting with a dot).
- `index.html` sends visitors on to the FlopShot pages.
- The app IDs are team `YYVJMB26A3` plus each build's bundle ID (Release, Beta, Dev). Add one here if a new build appears.
