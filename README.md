# Gold-Web website

The landing page for [Gold-Web](https://github.com/mrfrenchguy23445/gold-web),
a gaming and privacy browser for the desktop.

One static page. No build step, no framework, no external requests. Open
`index.html` directly, or serve the folder:

```sh
python3 -m http.server 8000
# then open http://127.0.0.1:8000/
```

## Files

| File | What it is |
|---|---|
| `index.html` | The whole page |
| `style.css` | Page styles, on top of the tokens |
| `assets/tokens.css` | A copy of the browser's Gold UI tokens |
| `assets/goldweb.png` | The wordmark |
| `assets/ui.png` | A capture of the current browser window |
| `assets/favicon.svg` | The gold diamond, matching the browser's logo mark |

`assets/tokens.css` is a copy of `brand/gold-ui/tokens.css` from the browser
repo, kept so the site is one self-contained folder. If those tokens change,
re-copy them so the website keeps matching the browser.

## Publishing

Served by GitHub Pages from the repository root. All asset paths are relative,
so the site also works from any static host, or straight off disk.

## Editing

Keep the copy honest and specific, the same rule the browser's own interface
follows: say what something does, and what it doesn't. "Blocks known trackers",
not "makes you anonymous". No em-dashes, no superlatives, no emoji.
