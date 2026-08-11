# jimtsipoutas.com

Built output only — GitHub Pages serves this repo as-is at https://jimtsipoutas.com.

The source lives in `~/Projects/jimtsipoutas` (vinext + React + Three.js).
To publish a change:

```
cd ~/Projects/jimtsipoutas
npm run build:static          # → dist/static
rsync -a --delete --exclude .git dist/static/ ../jimtsipoutas-site/
cd ../jimtsipoutas-site && git add -A && git commit -m "…" && git push
```
