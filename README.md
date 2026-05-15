# LoTR Website

Project website for **LoTR (Logic-of-Thought Routing)** — a plug-and-play reasoning router for LLMs.

## Live site

After you enable GitHub Pages (see below), the site URL will look like:

`https://<your-username>.github.io/<repository-name>/`

## Local preview

```bash
cd "/scratch/gongzhiren/LoTR/papers/website"
python -m http.server 8080
```

Open:

`http://localhost:8080`

## Repository layout

- `index.html` — sections, tables, and experiment modules
- `styles.css` — theme, layout, responsive styles
- `script.js` — lightbox, nav highlight, interactive result panels
- `assets/` — figures exported from paper materials

## Open source & GitHub Pages

1. Create a **public** empty repository on GitHub (example name: `LoTR-website`).
2. From this directory, add the remote and push the `main` branch:

   ```bash
   cd "/scratch/gongzhiren/LoTR/papers/website"
   git remote add origin https://github.com/<your-username>/<repository-name>.git
   git branch -M main
   git push -u origin main
   ```

   Use SSH instead of HTTPS if that is how you authenticate.

3. In the GitHub repo: **Settings → Pages → Build and deployment**.
   - **Source**: Deploy from a branch.
   - **Branch**: `main`, folder **`/ (root)`**.
   - Save and wait a few minutes for the first build.

4. Confirm the published URL loads; if Actions are enabled, check the **Pages** deployment run for errors.

Figures under `assets/` are included so the Pages site loads without referencing paths outside this repo.

## License

Licensed under the [MIT License](LICENSE).
