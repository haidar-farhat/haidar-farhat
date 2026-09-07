# Profile setup

This repository is the GitHub profile README for `haidar-farhat/haidar-farhat`.
Everything renders from `README.md`; the SVGs in `assets/` are static files and
need no build step.

## 1. Push and let the snake generate itself

The workflow in `.github/workflows/snake.yml` runs on the first push of the
workflow file, then daily at 03:17 UTC, and on demand from the **Actions** tab.
It writes two SVGs (light and dark) to an `output` branch, which the README
references directly:

```
https://raw.githubusercontent.com/haidar-farhat/haidar-farhat/output/github-contribution-grid-snake.svg
https://raw.githubusercontent.com/haidar-farhat/haidar-farhat/output/github-contribution-grid-snake-dark.svg
```

If GitHub asks, allow workflows under **Settings → Actions → General** and make
sure **Workflow permissions** is set to *Read and write* so the job can push the
`output` branch. Until the first run finishes the snake image is a broken link;
that resolves itself within a minute or two of the run.

## 2. Links to double-check

- The LinkedIn button points at `linkedin.com/in/haydar-farhat7`. Change it in
  the two places it appears in `README.md` if the handle is different.
- No email address is published on purpose. Add one to the **Let's Build
  Something** section if you want direct contact.

## 3. Pin repositories

The **Pinned** area on the profile page is separate from the README. Pin, in
this order, to match the featured cards:

1. `V.I.G.I.L._Vision_Intelligence_and_Geospatial_Incident_Layer`
2. `jobbler`
3. `Brevet-gpt`
4. `NU_Scaler`
5. `PhotoMaster`
6. `sm4rt_w4tch`

## 4. Profile bio and repository description

Suggested profile bio (Settings → Public profile):

> AI Engineer · computer vision, geospatial intelligence, LLM agents. I build local-first systems end to end: Python, Rust, TypeScript, Laravel.

Suggested description for this repository:

> AI Engineer building local-first vision, geospatial and LLM systems, end to end.

## 5. Stats cards

The stats, top-languages and streak cards are served by public instances
(`github-readme-stats.vercel.app`, `streak-stats.demolab.com`). The stats
instance is occasionally rate-limited and returns an error image for a few
minutes. If that becomes annoying, deploy your own copy of
[github-readme-stats](https://github.com/anuraghazra/github-readme-stats#deploy-on-your-own)
to Vercel and replace the host in the four `github-readme-stats.vercel.app`
URLs.

## 6. The SVG panels

Every section of the README is a hand-built animated SVG in `assets/`
(banner, section headers, profile, architecture, four project cards, stack,
timeline, uplink). They use only CSS and SMIL animation, no external fonts or
scripts, so GitHub renders them as-is. The design is deliberately dark-only;
the panels read as cards on both GitHub themes.

To change copy, edit the text inside the relevant SVG directly. The palette
tokens are the hex values at the top of each file's `<style>` block.

## 7. Social preview

Export `assets/banner.svg` to a 1280×640 PNG and upload it under
**Settings → Social preview** so the profile repository shares well.
