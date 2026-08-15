# Do not open these files directly in a browser

This folder contains **Jekyll source files** — they use `{{ }}` and `{% %}`
template syntax that only Jekyll (or GitHub Pages) can process. Opening
`index.html` here directly in Firefox/Chrome will show broken, unstyled
markup, because the browser has no idea what `{% include topbar.html %}`
means.

## Want to just look at the site?

Use `taraflow-static-preview.zip` instead (delivered alongside this file).
Unzip it and double-click its `index.html` — that version has everything
already resolved into plain HTML/CSS and works in any browser, no install
needed.

## Want to deploy the real site?

1. Copy everything in this folder into the root of your
   `TARAflow.github.io` repository (replacing the old files).
2. Commit and push.
3. GitHub Pages detects the Jekyll site automatically and builds it —
   no config, no CI setup needed. Give it a minute, then check
   `https://taraflow.github.io`.

## Want to preview the real build locally before pushing?

You need Ruby + Jekyll installed:

```
bundle exec jekyll serve
```

Then open `http://localhost:4000` — this is the only way to see the
*actual* Jekyll build (not the static-preview snapshot) without pushing
to GitHub first.
