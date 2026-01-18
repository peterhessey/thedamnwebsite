# Website

The repo for my website. Inspired by [this post from Louie Mantia Jr.](https://lmnt.me/blog/how-to-make-a-damn-website.html) after too many attempts at getting bogged down in static site generators before losing interest.

## Usage

Write posts in `md` and convert posts from `md` to `html` with:

```shell
for f in posts/md/*.md; do pandoc "$f" -s --css ../../style.css -o "posts/html/$(basename "${f%.md}").html"; done
```
