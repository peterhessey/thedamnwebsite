# Website

The repo for my website. Inspired by [this post from Louie Mantia Jr.](https://lmnt.me/blog/how-to-make-a-damn-website.html) after too many attempts at getting bogged down in static site generators before losing interest.

## Usage

[Install `pandoc`](https://pandoc.org/installing.html) and convert posts from `md` to `html` with:

```shell
for f in md/*.md; do pandoc "$f" -o "html/$(basename "${f%.md}").html"; done
```
