maybe automate wiki home page generation? use github actions [see](https://spinscale.de/posts/2021-10-29-github-actions-updating-github-wiki-after-edit.html)

for each file do `git log -1 --pretty="format:%cs"` and build home.md, commit that
