# dhanush788.github.io

Personal portfolio — [dhanush788.github.io](https://dhanush788.github.io)

## Layout

```
index.html              the whole site (no build step, no dependencies)
404.html                not-found page
resume/resume.tex       résumé source
resume.pdf              compiled by CI, served at /resume.pdf
CNAME                   custom domain
```

## Editing

`index.html` is self-contained — markup, CSS tokens and a small script in one file.
Change the content, commit to `main`, and GitHub Pages redeploys in ~60 seconds.

Colours live in the `:root` / `[data-theme="light"]` token blocks at the top of
the `<style>` element. Change `--accent` in both to re-skin the site.

## Résumé

Edit `resume/resume.tex` and push. The
[workflow](.github/workflows/resume.yml) compiles it with `pdflatex` and
commits the result to `resume.pdf` at the repo root, so the download button
always serves the current version. Run it manually from the Actions tab with
**Build resume PDF → Run workflow**.
