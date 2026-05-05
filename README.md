# hone-landing

Temporary coming-soon landing page for [hone.study](https://hone.study).

This is throwaway code. The real app — an open source AI-native learning toolkit — will replace this by pointing the domain at a different repo.

## Contents

- `index.html` — the entire page (HTML + CSS + a small bit of vanilla JS)

No build step, no dependencies, no `package.json`.

## Running locally

Just open `index.html` in a browser, or serve the directory:

```sh
python3 -m http.server 8000
# then visit http://localhost:8000
```

## Deploying

### Cloudflare Pages

1. Go to Cloudflare Pages → Create a project → Direct Upload
2. Drag the repo folder in
3. Point the `hone.study` domain at the project

Or connect the GitHub repo and let it auto-deploy on push (no build command, output directory `/`).

### Vercel

```sh
npx vercel deploy --prod
```

No config needed — Vercel serves `index.html` from the repo root.

## TODO before launch

- Wire the email form to a real provider (Buttondown or Kit). Search `index.html` for `TODO` to find the spot.
