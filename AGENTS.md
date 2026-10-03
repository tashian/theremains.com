Hugo site for https://theremains.com (the band The Remains). Pushes to GitHub (`tashian/theremains.com`). A GitHub Actions workflow (`.github/workflows/hugo.yml`) builds `main` and deploys it to GitHub Pages.

- Local preview: `hugo server`
- Build: `hugo --gc --minify` (output in `public/`)
- Pages are in `content/`. Shows are in `content/shows/`: one file per show. The Shows page sorts them into upcoming and past by `date`.
- Images are in `static/images/`. The home page audio file is `static/audio/time-of-day.mp3`.
- The site came from Squarespace in October 2026. Show pages keep their old Squarespace URLs through the `url` front matter key. Do not change these URLs. `/home` redirects to `/` through a Hugo alias.
- DNS for theremains.com is in AWS Route 53. The registrar is Namecheap. Email uses Google Workspace MX records, so keep the MX records when you change DNS.
- The GitHub Pages custom domain is `theremains.com` (apex). GitHub Pages redirects `www.theremains.com` to the apex domain because `www` is a CNAME to `tashian.github.io`.
