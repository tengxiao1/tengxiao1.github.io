# tengxiao1.github.io

Source for [tengxiao1.github.io](https://tengxiao1.github.io/). Static HTML + CSS, no build step —
GitHub Pages serves `index.html` directly, so any push to `master` goes live in a minute or two.

## Files

| Path | What it is |
| --- | --- |
| `index.html` | All page content: bio, news, publications, service |
| `stylesheet.css` | All styling, including the light/dark palettes |
| `images/favicon/` | Favicons |
| `images/profile.jpg` | Your portrait — add this file and the page picks it up |

## Editing

**Photo.** Save a square image as `images/profile.jpg`. Until it exists the page falls back to
`images/profile.svg`, a generic placeholder.

**News.** Copy one `<li>` inside `<ul class="news">`, newest first. The list scrolls past ~6 entries,
so old items can stay.

**Publications.** Each paper is one `<li class="pub">` inside the `<ol class="pubs">` for its year.
Wrap your own name in `<span class="me">Teng Xiao</span>` and equal-contribution marks in
`<span class="star">*</span>`. The venue chip takes a colour from its second class —
`venue-neurips`, `venue-icml`, `venue-iclr`, `venue-colm`, `venue-emnlp`, or `venue-preprint`.
Add `<span class="award">Oral</span>` after the title for a highlight.

## Preview locally

```
python3 -m http.server 8000
```

Then open <http://localhost:8000>.
