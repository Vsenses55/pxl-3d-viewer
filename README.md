# PXL 3D Viewer

An interactive Three.js viewer for the PXL logo 3D asset — drag to rotate, scroll to zoom, coral-to-peach gradient studio backdrop matching the reference render.

## Files

- `index.html` — the viewer (Three.js, loaded from a CDN via import map)
- `pxl_logo.glb` — the exported 3D model (glTF binary)

## Running it locally

Open `index.html` in a browser. Note: some browsers block loading local `.glb` files directly from disk (`file://`), so if it doesn't load, serve the folder locally instead, e.g.:

```
python3 -m http.server 8000
```

then visit `http://localhost:8000`.

## Hosting on GitHub Pages

Once this repo is on GitHub:

1. Go to the repo's **Settings** tab → **Pages** (left sidebar).
2. Under "Build and deployment", set **Source** to "Deploy from a branch".
3. Set **Branch** to `main` and folder to `/ (root)`, then **Save**.
4. GitHub will publish the site at `https://<your-username>.github.io/<repo-name>/` within a minute or two.
