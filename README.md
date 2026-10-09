# Baitul Aman Jame Masjid

Static mosque website with Home, About, Services, Timetables, Gallery and Donate pages. The gallery has ten captioned albums and rotating photo reels. The homepage crowd reel advances every five seconds.

## Preview

Run `python3 -m http.server 8765 --directory dist` from this folder.

## Publish

GitHub Actions deploys `dist/` to GitHub Pages when main is pushed. Configure Pages to use GitHub Actions, and set the custom domain to `www.baitul-aman.com`.

Namecheap DNS: www CNAME points to your GitHub username followed by `.github.io`. Add four A records for @: 185.199.108.153, 185.199.109.153, 185.199.110.153 and 185.199.111.153. Preserve email records. Once DNS resolves and GitHub issues the certificate, enable Enforce HTTPS in Pages settings.

## Content updates

Edit HTML, CSS and JavaScript in dist. Prayer data contains supplied January–October 2026 times; November and December are unavailable until supplied. Add new records and their PDFs together. Dates use Europe/London time.

Online donation buttons currently display Coming Soon. Stripe hosted payment links can be added later without a database or custom backend.
