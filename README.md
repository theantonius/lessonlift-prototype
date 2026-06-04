# LessonLift demo site

One folder, four sections, no backend. Drag this whole `lessonlift_site` folder onto https://app.netlify.com/drop to get a temporary public URL.

## What's inside

- `index.html` — landing hub linking to the four demos.
- `prototype/` — the clickable teacher prototype (analyze → report → annotations → plan).
- `bundles/` — a page that plays the bundles-and-sticks detection clip.
- `handtracking/` — live, in-browser hand tracking using your webcam. On-device.
- `figma/` — placeholder page; paste your Figma share link into `figma/index.html`.

## Before you publish

- The live hand tracking needs **https** for the webcam. Netlify gives you https automatically, so it works there. It will not work from a `file://` path opened directly.
- The hand-tracking demo asks for camera permission and runs entirely on the viewer's device. No video is uploaded.
- Confirm the prototype's `finger_counting.mp4` shows no identifiable student before publishing publicly. The bundles clip is manipulatives and is fine.
- Set the Figma link: open `figma/index.html` and replace `REPLACE_WITH_FIGMA_LINK` with your Figma share URL.
