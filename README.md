# LessonLift demo site

A static demo of LessonLift. One repo, four sections, no backend or build step.
Built at Multilingual by Design Design Days (June 2-4, 2026) by Integrow Math
Solutions and NYC FIRST.

## What's inside

- `index.html` — landing hub linking to the four demos.
- `prototype/` — the clickable teacher prototype (analyze → report → annotations → plan).
- `bundles/` — a page that plays the bundles-and-sticks detection clip.
- `handtracking/` — live, in-browser hand tracking using your webcam. Runs on-device.
- `figma/` — placeholder page; paste your Figma share link into `figma/index.html`.

## Hosting

This repo is deployed with **Cloudflare Pages**, connected to the GitHub repo.

- Every push to `main` triggers an automatic redeploy. To update the live site,
  just commit and push:
  ```
  git add .
  git commit -m "what changed"
  git push
  ```
- First-time setup (already done): Cloudflare dashboard → Workers & Pages →
  Create → Pages → Connect to Git → pick this repo. Framework preset **None**,
  build command empty, build output directory `/` (root).

## Notes

- The live hand tracking needs **https** for the webcam. Cloudflare Pages serves
  https, so it works there. It will not work from a `file://` path opened directly.
- The hand-tracking demo asks for camera permission and runs entirely on the
  viewer's device. No video is uploaded.
- Confirm `prototype/clips/finger_counting.mp4` shows no identifiable student, since
  this is a public site. The bundles clip is manipulatives and is fine.
- Set the Figma link: open `figma/index.html` and replace `REPLACE_WITH_FIGMA_LINK`
  with your Figma share URL.
