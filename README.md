# benjaminsirb.com

Personal CV site. One static page, no build step, hosted on GitHub Pages at https://benjaminsirb.com.

## Files

- `index.html`: the whole site (HTML, CSS and a few lines of JS in one file). Edit this.
- `option-a.html`: an earlier single-column layout, kept for reference. Not linked anywhere.
- `CNAME`: the custom domain. Do not remove it, or Pages drops the domain.
- `.nojekyll`: tells Pages to serve the files as they are.

## How to edit

1. Edit `index.html`. Each section is marked with `<section id="...">`.
   - Experience: one `<article class="job">` per employer, bullets in a `<ul>`.
   - Publications: one `<li>` per paper in `<ul class="pubs">`. To link a paper, wrap the title: `<a href="https://arxiv.org/abs/...">Title</a>`, and put the venue in the `<span class="venue">`.
   - Skills: one `<span class="pill">` per item.
2. Open the file in a browser to check it (`open index.html`).
3. Commit and push to `main`. Pages rebuilds in about a minute.

```bash
git add -A && git commit -m "Add publication" && git push
```

## Domain and HTTPS

DNS lives in Squarespace: four A records for `@` pointing at GitHub Pages (185.199.108.153 to 185.199.111.153) and a CNAME for `www` to `benjaminsirb.github.io`. HTTPS is enforced in the repo's Settings, Pages, once GitHub has issued the certificate.
