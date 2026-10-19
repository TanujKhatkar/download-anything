# Download Anything — website

Static pages for GitHub Pages. Two files, no build step, no dependencies.

- `index.html` — landing page: what it does, screenshots, install steps, FAQ
- `privacy.html` — privacy policy (use this URL in the Chrome Web Store "Privacy policy URL" field)

## Publish on GitHub Pages

1. Create a public repository, e.g. `download-anything`.
2. Upload everything in this folder to the repository root (keep the `assets/` folder).
3. Repository **Settings → Pages** → Source: **Deploy from a branch** → Branch: **main**, folder **/ (root)** → **Save**.
4. Wait about a minute. Your URLs will be:

```
https://YOUR-USERNAME.github.io/download-anything/
https://YOUR-USERNAME.github.io/download-anything/privacy.html
```

Paste the second URL into the Chrome Web Store dashboard → Privacy → **Privacy policy URL**.
Put the first one in Store listing → Additional fields → **Homepage URL**, and
`https://github.com/YOUR-USERNAME/download-anything/issues` as the **Support URL**.

## Before publishing

Replace the placeholder email in `privacy.html` (section 12) with your real address.

## Notes

- `.nojekyll` is included so GitHub serves the files as-is.
- `assets/download-anything-1.0.0.zip` is the full package (extension + engine).
- If you publish a new build, drop the new zip in `assets/` and update the two
  `href` values in `index.html` and the one in `privacy.html`.
