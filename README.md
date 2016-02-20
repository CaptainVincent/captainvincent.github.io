# captainvincent.github.io
Personal Blog

How to convert localhost link to github site.
```bash
find static -name "*.html" -exec sed -i .sedbak 's/localhost:2368/captainvincent.github.io/g' '{}' \;
```