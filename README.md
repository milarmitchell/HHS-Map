# Hinkley CLDE Resources

A small multi-page static site — plain HTML/CSS, no build tools, ready for GitHub Pages.

## Structure

```
hinkley-clde-resources/
├── index.html                        ← home page (resource directory)
├── map/
│   └── index.html                    ← floor plan finder (currently a placeholder — see below)
└── academic-conversations/
    └── index.html                    ← academic conversation skill posters
```

Each resource lives in its own folder with an `index.html` inside, so it gets a clean URL:
`yourusername.github.io/repo-name/map/` and `yourusername.github.io/repo-name/academic-conversations/`.

## Floor plan finder

`map/index.html` is your real floor plan finder — the nav bar has been added on top of it, and the rest of the file (search, floor tabs, room data) is untouched.

## Adding a new resource later

1. Create a new folder, e.g. `writing-frames/`, with an `index.html` inside.
2. Copy the `<header class="site-nav">` block from any existing page into it, and add a link to the new page in every page's nav (including the new one).
3. Add a matching card to the grid in the root `index.html`.

## Hosting on GitHub Pages

If Pages is already enabled on this repo (Settings → Pages → deploy from a branch), pushing this structure to that branch's root is all that's needed — no config changes.

If you'd like the site's URL slug itself to say "hinkley-clde-resources" rather than the map project's old name, rename the repository: Settings → General → Repository name. This only changes the URL path after your GitHub username; it doesn't affect anything inside the repo.
