# tengxiao1.github.io

Source for [tengxiao1.github.io](https://tengxiao1.github.io/). Static HTML + CSS, no build step —
GitHub Pages serves `index.html` directly, so any push to `master` goes live in a minute or two.

## Files

| Path | What it is |
| --- | --- |
| `index.html` | All page content: bio, news, publications, service |
| `stylesheet.css` | All styling; dark mode follows the system setting |
| `images/favicon/` | Favicons |
| `images/profile.jpg` | Your portrait — add this file and the page picks it up |

## Editing

**Photo.** Save a square image as `images/profile.jpg`. Until it exists the page falls back to
`images/profile.svg`, a generic placeholder.

**News.** Copy one `<li>` into the first `<ul class="news">`, newest first. Keep about six there and
move older items into the list inside `<details class="more">`, which is folded under "More news".

**Publications.** Each paper is one `<li class="pub">` inside the `<ul class="pubs">` under its theme
(`<h3>`). An entry is a title link, an authors line and a meta line:

```html
<li class="pub">
  <a class="title" href="PAPER_URL">Title</a>
  <div class="authors">A. Author*, <b class="me">Teng Xiao</b>*, B. Author</div>
  <div class="meta"><span class="venue">ICLR 2025</span><span class="award">Oral, top 1.8%</span><span class="links"><a href="PAPER_URL">Paper</a><a href="CODE_URL">Code</a></span></div>
  <p class="impact">One line on why the paper matters, with <strong>key numbers</strong> in bold.</p>
</li>
```

Use `<span class="venue pre">` for preprints and tech reports (set in grey). `award` and `impact` are
optional. They are the only blue text on the page, so keep them for the papers you want to stand out.

## Preview locally

```
python3 -m http.server 8000
```

Then open <http://localhost:8000>.
