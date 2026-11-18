# Personal website

A one-page site, with no build step. All files live in this folder:

| File         | What it is                                                                 |
|--------------|----------------------------------------------------------------------------|
| `index.html` | The whole site: content, styles, and the small paper-filter script         |
| `cv.pdf`     | Compiled from `Apps/Overleaf/CV/cv_chu.tex` (November 18, 2026)            |
| `photo.jpg`  | Headshot, cropped to 4:5 (367×459 px) from `Non-Research/Other Documents/dr_chu_headshot.jpg`. A larger original (800 px wide or more) would look sharper on high-resolution screens. |

## Updating

- **New working paper:** copy any `<li class="paper" ...>` block under `id="wp-list"` and edit it. The `data-topics` attribute controls which topic chips match it. Use any of `banking housing politics corporate inequality climate ai pricing`.
- **Paper accepted:** move its block to `pub-top` or `pub-other`, add `data-year="2026"` (or `"forthcoming"`), and put the year in the `<div class="gutter">`. Keep each list sorted newest first.
- **R&R status:** put it in the gutter, e.g. `<div class="gutter status">R&amp;R · JFQA</div>`.
- **New CV:** overwrite `cv.pdf`, then update the month in the CV button text ("November 2026").
- Update the counts in the headings (17 / 36 / 11 / 25) when you add papers. The script corrects them on load, but search engines read the HTML.

## Hosting options

1. **GitHub Pages (recommended, free).** Create a repo named `<username>.github.io`, upload these files, and the site is live at `https://<username>.github.io`. You can point a custom domain such as `yongqiangchu.com` at it.
2. **University web space**, if Belk College offers faculty pages that accept HTML uploads.
3. **Stay on Google Sites.** It cannot host this file directly. You can rebuild the same structure there with its own blocks, but the topic filter and the layout control will not carry over.

The site is live at https://yongqiangchufinance.github.io (repository `yongqiangchufinance/yongqiangchufinance.github.io`, in the free `yongqiangchufinance` GitHub organization owned by your personal account). The CV sources in `Apps/Overleaf/CV` and the old Google Site point here.
