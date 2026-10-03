Hugo site for https://theremains.com (the band The Remains). Pushes to GitHub (`tashian/theremains.com`); Vercel deploys `main` from there.

- Local preview: `hugo server`
- Build: `hugo --gc --minify` (output in `public/`)
- Pages are in `content/`. Shows are in `content/shows/`: one file per show. The Shows page sorts them into upcoming and past by `date`.
- Images are in `static/images/`. The home page audio file is `static/audio/time-of-day.mp3`.
- The site came from Squarespace in October 2026. Show pages keep their old Squarespace URLs through the `url` front matter key. Do not change these URLs.
- DNS for theremains.com is in AWS Route 53. The registrar is Namecheap. Email uses Google Workspace MX records, so keep the MX records when you change DNS.
- `https://www.theremains.com` redirects to the apex domain. Vercel controls this redirect in the project domain settings.
