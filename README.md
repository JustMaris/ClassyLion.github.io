# JustMaris.github.io

Source for **[maris.popens.eu](https://maris.popens.eu/)** — my personal landing page.

A single hand-written `index.html` + `css/style.css`. No build step, no JavaScript,
no trackers. Light and dark themes follow the system preference.

## Deploy

GitHub Pages, served from the `master` branch at `/` (root). Pushing to `master`
redeploys. Custom domain via `CNAME`.

## Blog list

The "From the blog" section is kept between `<!-- BLOG-POSTS:START -->` and
`<!-- BLOG-POSTS:END -->` markers in `index.html`. `.github/workflows/update-blog.yml`
runs `scripts/update_blog.py` daily to refresh it from the
[drumandbytes.com](https://drumandbytes.com/) RSS feed and commits any change back
to `master`. Run it by hand from the Actions tab, or:

```
python3 scripts/update_blog.py
```
