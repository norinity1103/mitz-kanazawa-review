# Mitz Kanazawa Domain Launch Checklist

## Target Domain

- Primary domain: `mitz-kanazawa.com`
- GitHub Pages repository: `norinity1103/mitz-kanazawa-review`
- Published branch: `main`

## GitHub Pages

1. Open repository settings.
2. Go to `Settings` -> `Pages`.
3. Confirm `Custom domain` is `mitz-kanazawa.com`.
4. After DNS propagation, enable `Enforce HTTPS`.

## DNS

Set the apex domain to GitHub Pages.

```txt
mitz-kanazawa.com. A 185.199.108.153
mitz-kanazawa.com. A 185.199.109.153
mitz-kanazawa.com. A 185.199.110.153
mitz-kanazawa.com. A 185.199.111.153
```

If `www.mitz-kanazawa.com` is used, add:

```txt
www.mitz-kanazawa.com. CNAME norinity1103.github.io.
```

## Post Launch Checks

- `https://mitz-kanazawa.com/` returns `200`.
- `https://mitz-kanazawa.com/CNAME` returns `mitz-kanazawa.com`.
- `https://mitz-kanazawa.com/robots.txt` returns the sitemap URL.
- `https://mitz-kanazawa.com/sitemap.xml` returns the production URL.
- OGP image resolves at `https://mitz-kanazawa.com/images/ogp-grand-open.jpg`.
- Sponsor PDF resolves at `https://mitz-kanazawa.com/assets/Mitz_Sponsorship_2026.pdf`.
