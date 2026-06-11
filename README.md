# Rad Hats for Rad Humans

Static site, no build step. One page: `index.html` + `hats.js` (the 50 hats data) + `assets/` (site photos) + `photos/` (individual hat photos).

## Deploy (one time setup)

1. Create an empty GitHub repo `ssaitsky/radhats`.
2. From this folder: `git remote add origin https://github.com/ssaitsky/radhats.git && git push -u origin main`
3. In Vercel: Add New Project → import `ssaitsky/radhats` → deploy (no settings needed, it is plain HTML).
4. In Vercel project settings → Domains → add `radhatsforradhumans.com`, then update the domain's DNS as Vercel instructs (A record 76.76.21.21 or move nameservers).

After that, every push to `main` auto-deploys.

## Updating the hats

- Names and stories live in `hats.js`. Edit text there.
- Real hat photos: drop files named `hat-01.jpg` ... `hat-50.jpg` into `photos/`. Each one automatically replaces that hat's placeholder illustration. See `photos/README.md`.

## Site photos

`assets/` holds the 6 images rescued from the old GoDaddy site (logo, hero portrait, Svet and Rad, Rad in his hat, the 16 hat collage, order section photo).
