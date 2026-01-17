# Website

The repo for my website.

## Usage

[Install `pandoc`](https://pandoc.org/installing.html) and convert posts from `md` to `html` with:

```shell
for f in md/*.md; do pandoc "$f" -o "html/$(basename "${f%.md}").html"; done
```
