# [ADDRESS] — Luxury Listing Site

A single-property real estate brochure site, built with [Quartz](https://quartz.jzhao.xyz/) from an Obsidian vault and deployed automatically to GitHub Pages.

**Live site:** https://graciachase-dev.github.io/Real-Estate-Site/

## How the site is put together

- All page content lives in **one file**: `content/index.md`. Every section (hero, overview, gallery, features, floor plan, virtual tour, location, contact, footer) is HTML embedded directly in that markdown file.
- The visual design (fonts, colors, layout, animations, photo placeholder styling) lives in `quartz/styles/custom.scss`.
- Site-wide settings (page title, color palette, fonts, which sidebar/wiki features are on or off) live in `quartz.config.yaml`.

## Updating content

The source of truth is your **Obsidian vault**, not this repo directly:

```
~/Desktop/Obsidian/Tutorial-test/index.md
```

1. Open that file in Obsidian (or any text editor) and edit it.
2. Replace the bracket placeholders — `[ADDRESS]`, `[PRICE]`, `[BEDS]`, `[BATHS]`, `[SQFT]`, `[LOT SIZE]`, `[PLACEHOLDER PARAGRAPH]`, `[AGENT NAME]`, `[BROKERAGE]`, `[PHONE]`, `[EMAIL]`, `[MLS#]` — with real listing details. There's a comment block at the top of the file listing every token.
3. Copy the updated file into the Quartz project (content isn't symlinked, so this step is required after every edit):
   ```bash
   cp ~/Desktop/Obsidian/Tutorial-test/index.md ~/quartz/content/index.md
   ```
4. Commit and push (see below) to publish the change.

## Swapping in real photos

Every photo/floor-plan/video slot is currently a placeholder `<div class="photo-placeholder">` (or `<button class="photo-placeholder ll-photo">` in the gallery) with a `data-label` describing exactly which photo goes there, e.g. `"Exterior — Front Facade"`.

To swap one in:

```html
<!-- before -->
<button class="photo-placeholder ll-photo" data-label="Exterior — Front Facade" type="button">
  <svg class="ph-icon" ...>...</svg>
  <span class="ph-label">Exterior — Front Facade</span>
</button>

<!-- after -->
<button class="photo-placeholder ll-photo" type="button">
  <img src="images/exterior-front.jpg" alt="Exterior — Front Facade" loading="lazy" />
</button>
```

The surrounding container already has the correct aspect ratio set in `custom.scss`, so this is a drop-in replacement — no layout or CSS changes needed. Put image files in `content/images/` (create the folder) and reference them with a relative path.

For the **virtual tour**, replace the placeholder in the Virtual Tour section with a real `<iframe>` (a commented-out Matterport example is right above it in the markdown). For the **map**, replace the `q=[ADDRESS]` value in the Location section's iframe `src` with the real address — no API key needed.

## Deployment (GitHub Pages)

This repo auto-deploys on every push to `main` via GitHub Actions (`.github/workflows/deploy.yml`):

1. Checks out the repo
2. Installs dependencies (`npm ci`)
3. Installs Quartz's plugin ecosystem (`npx quartz plugin install`) — required because `.quartz/plugins/` is gitignored and gets regenerated from `quartz.lock.json`
4. Builds the site (`npx quartz build`)
5. Publishes the `public/` output to GitHub Pages

To publish a change:

```bash
cd ~/quartz
git add -A
git commit -m "Update listing content"
git push
```

Then check the **Actions** tab on GitHub for a green checkmark. The live site updates within a minute or two of a successful run.

## Previewing locally before you push

```bash
cd ~/quartz
npx quartz build --serve
```

Then open http://localhost:8080 in a browser. Press `Ctrl+C` in the terminal to stop the preview server.
