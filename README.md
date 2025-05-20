# JBL pdf.js

To get the latest pdf.js version published on our gh-pages
1. Sync `master` with the upstream
2. Imitate `publish_release.yml` workflow logic and:
  - Locally run `npx gulp web`
  - Grab compiled static page at `build/gh-pages`
3. Commit the latest static page to a new branch `gh-pages-X`
4. Apply custom patches (if relevant)
5. Deploy your `gh-pages-X` branch using [github pages](https://github.com/jobylon/pdf.js/settings/pages)