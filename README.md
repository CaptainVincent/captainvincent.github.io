# captainvincent.github.io
Personal Blog

How to convert localhost link to github site.
```bash
find static -name "*.html" -exec sed -i .sedbak 's/localhost:2368/captainvincent.github.io/g' '{}' \;
find static/how-to-setup-ghost-blog-platform-shang -name "*.html" -exec sed -i .sedbak 's/captainvincent.github.io/localhost:2368/g' '{}' \;
find static -name "robots.txt" -exec sed -i .sedbak 's/localhost:2368/captainvincent.github.io/g' '{}' \;
find static -name "*.rss" -exec sed -i .sedbak 's/localhost:2368/captainvincent.github.io/g' '{}' \;
find static -name "*.sedbak" | xargs rm -rf
```
