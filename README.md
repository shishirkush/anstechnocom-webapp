# ANS Technocom — anstechnocom.in

Marketing / recruitment site for ANS Technocom's work-from-home telecalling
program (credit card sales, on top of the [telecalling-app](https://github.com/shishirkush/telecalling-app)
Android app and Supabase backend).

Single static file, no build step — zero-cost hosting on GitHub Pages.

```
index.html   the whole site
CNAME        custom domain for GitHub Pages (anstechnocom.in)
```

## Deploy

Pushes to `master` publish automatically via GitHub Pages once Pages is
enabled on this repo (Settings → Pages → Source: Deploy from a branch →
`master` / `/ (root)`).

## Custom domain (anstechnocom.in)

At your domain registrar, point the apex domain at GitHub Pages:

**A records** for `@` (root domain) → all four GitHub Pages IPs:
```
185.199.108.153
185.199.109.153
185.199.110.153
185.199.111.153
```

**CNAME record** for `www` →
```
shishirkush.github.io
```

DNS changes can take a few hours to propagate. Once they resolve, GitHub
Pages will issue an HTTPS certificate for anstechnocom.in automatically
(Settings → Pages → Enforce HTTPS, once the certificate is ready).
