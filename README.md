# mizukislove.github.io

Personal website of Qinglang Liao, built with [Quarto](https://quarto.org). Every push to `main` rebuilds and publishes the site automatically (see `.github/workflows/publish.yml`).

## Where things are

| File | Page |
| --- | --- |
| `index.qmd` | About (home page) |
| `research.qmd` | Research |
| `publications.qmd` | Publications and presentations |
| `writing.qmd` + `posts/` | Writing (blog) |
| `code.qmd` | Code |
| `beyond.qmd` | Beyond research |
| `cv.qmd` | CV |
| `_quarto.yml` | Site title, menu, colours |

Pages with `draft: true` at the top are hidden from the live site. Delete that line to publish the page.

## Common edits

**Fix a typo or change text (in the browser):** open the file on github.com, click the pencil icon, edit, and click "Commit changes". The site updates in about two minutes.

**Add a post with no R code (in the browser):** in `posts/`, click "Add file" → "Create new file", and name it `posts/my-post-name/index.qmd`. Paste the contents of `_post-template/index.qmd`, edit, and delete the `draft: true` line when it's ready.

**Add a post with R code (in RStudio):**
1. Copy `_post-template/` to `posts/my-post-name/` and write the post.
2. Click Render. This runs the code and saves the results in `_freeze/`.
3. Commit and push everything, including `_freeze/`. The website uses the saved results, so R does not have to run on GitHub.

**Add your photo:** save it as `images/profile.jpg` and change `image: images/avatar.svg` in `index.qmd` to `image: images/profile.jpg`.

**Add your CV PDF:** save it as `files/cv.pdf` (leave out your phone number), then uncomment the CV lines in `index.qmd` and `cv.qmd`.

**Preview before publishing (in RStudio or a terminal):** run `quarto preview`.
