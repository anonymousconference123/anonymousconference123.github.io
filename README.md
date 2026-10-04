# LongContextVLA project website

A static, anonymous paper website. No installation, JavaScript, or build step is required.

## Preview

Open `index.html` in a browser, or run this command from this folder:

```sh
python3 -m http.server 8000
```

Then visit http://localhost:8000.

## Publish to GitHub Pages

1. Upload the **contents of this folder** to `anonymousconference123/anonymousconference123.github.io`. Put `index.html` at the repository root, not inside a `website` folder. Replace the existing README if desired.
2. Include `styles.css`, `paper.pdf`, `.nojekyll`, and both the `assets/` and `videos/` folders. The page uses relative paths and needs no configuration changes.
3. In the repository, open **Settings → Pages**.
4. Select **Deploy from a branch**, **main**, and **/ (root)**, then save.
5. After deployment, visit https://anonymousconference123.github.io/.

Use the anonymous account for commits and its GitHub-provided noreply email if uploading with Git. Do not copy the source project's Git history.

## Edit the content

- `index.html`: title, abstract, demonstration captions, method summary, and results.
- `styles.css`: typography, spacing, and responsive layout.
- `assets/`: figures cropped from the supplied paper, plus video poster images.
- `paper.pdf`: the supplied anonymous paper, unchanged.
- `videos/cup_mix.mp4`, `videos/drawer.mp4`, `videos/prompting_ood.mp4`: demonstration videos. Keep these paths when replacing videos.

The abstract is reproduced from the paper with its final project-website sentence removed. Numerical results are taken from Figure 4 and Table 1; the latency discussion comes from Figure 5 and Section 5. The video-prompting caption explains replacement of memory context with a demonstration and generalization from three to five objects, including two unseen object types. The RoboMME section includes every result row from Table 1, with human and oracle reference results clearly separated. Video-prompting results are shown separately from narration ablations, as in the paper.

Videos use H.264/AAC MP4 with fast-start metadata for browser playback. Video originals remain outside this website folder. Videos load only when requested, and each player has native playback, seeking, volume, and full-screen controls. Figures link to their full-size images.

The site uses local assets and system fonts, with no analytics or third-party embeds. Before publishing, review the supplied paper and videos for any identifying content you do not want made public.
