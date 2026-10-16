# Mitul Shahriyar — Personal Site

Personal website for Mitul Shahriyar: community work, events, talks, credentials, YouTube series and contact.

It is a single static page with no build step. Fonts load from Google Fonts.

## Files

| File | Purpose |
|------|---------|
| `index.html` | The whole site (HTML, CSS and JS in one file) |
| `favicon.svg` | Browser tab icon |
| `.nojekyll` | Tells GitHub Pages to serve files as-is |

## Deploy on GitHub Pages

1. Create a new repository on GitHub. Name it `mitul3737.github.io` to get the site at `https://mitul3737.github.io`, or use any name (e.g. `portfolio`) to get `https://mitul3737.github.io/portfolio`.
2. Push these files:
   ```bash
   git init
   git add .
   git commit -m "Launch personal site"
   git branch -M main
   git remote add origin https://github.com/mitul3737/<repo-name>.git
   git push -u origin main
   ```
3. In the repository, open **Settings → Pages**.
4. Under **Build and deployment**, set **Source** to *Deploy from a branch*, choose `main` and `/ (root)`, and save.
5. Wait a minute or two. The live URL appears at the top of the Pages settings.

## Custom domain (optional)

1. Add a file named `CNAME` containing only your domain, e.g. `mitulshahriyar.com`.
2. At your domain registrar, add a `CNAME` record pointing `www` to `mitul3737.github.io`, or `A` records for the apex domain pointing to GitHub's Pages IPs (185.199.108.153, 185.199.109.153, 185.199.110.153, 185.199.111.153).
3. In **Settings → Pages**, enter the domain and turn on **Enforce HTTPS**.

## Updating content

- **Events:** edit the `events` list near the bottom of `index.html`. Each entry has a date (`d`, as `YYYY-MM-DD`), title (`t`), meta line (`m`) and description (`x`). Upcoming and past are sorted automatically by today's date.
- **Colors:** change the tokens in the `:root` block at the top of the `<style>`. The dark-mode values are in the two blocks right after it.
- **Email links:** the contact section shows the address with a copy button. On your own domain, `mailto:` links work normally, so you can wrap the address in `<a href="mailto:mitulshahriyar@gmail.com">` if you like.
