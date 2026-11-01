# Surf Collective India — website starter

A responsive, static website inspired by the cinematic surf-camp aesthetic of the supplied reference. It is an original layout and copy, not a copy of Flow State Bali.

## Preview locally
Open `index.html` in a browser, or run a local server from this folder:
`python3 -m http.server 8000`
Then visit http://localhost:8000

## Personalise the hero image
In `styles.css`, replace the background image URL in `.hero-image` with your uploaded image URL or a file path such as `assets/hero.jpg`.
Also replace the matching image in the `.image-ribbon` section of `index.html` if desired.
Put local image files in `assets/`.

## Add your videos
Open `script.js` and replace the empty values in:
`const videos={wave:'',surfskate:''};`
with hosted MP4 URLs or YouTube/Vimeo links. For local MP4 files, put them in `assets/` and use `assets/wave.mp4` / `assets/surfskate.mp4`.
Use video files you own or have permission to publish.

## Update imagery
The starter uses remote Unsplash image URLs as temporary stock imagery. Replace them with your own photos for the final brand website.

## Free hosting
### Cloudflare Pages (recommended)
1. Create/sign in to a Cloudflare account.
2. Open Workers & Pages → Create → Pages → Upload assets (or connect a Git repository).
3. Upload the contents of this folder (the `index.html`, `styles.css`, `script.js`, and `assets` folder).
4. Choose the project name `surfcollective` if available. Cloudflare will provide `https://surfcollective.pages.dev` if that project name is available; otherwise it will suggest an available name.
5. For Git deployment, push these files to a GitHub repository and connect it to Pages. Framework preset: None; build command: leave blank; output directory: `/`.

### Vercel alternative
Import the GitHub repository into Vercel. Choose Other as framework preset, no build command, and `.` as output directory. Vercel provides a `*.vercel.app` address.

A hosting account login/authorisation is required to publish. This project has not been deployed from this package.


## Surf Collective media included
- `assets/surfcollective-hero.jpg`: your beach/surfer photo, used as the homepage hero and intro image.
- `assets/wave-catching.mp4`: 30-second surf edit, plays as a live preview on the Wave Chasers card and behind the manifesto section.
- `assets/surfskate-turns.mp4`: 30-second surfskate edit, plays as a live preview on the Carve & Flow card.
- Clicking either card opens the full video with sound.
- `assets/culture-lesson.jpg` and `assets/strip-*.jpg`: photos from your own footage (replaced the stock images).

Keep the `assets/` folder next to `index.html` when deploying.

## Deploy with GitHub + Vercel
1. github.com → New repository → name `surfcollective` → Public → Create.
2. Click "uploading an existing file", drag in everything inside this folder (index.html, styles.css, script.js, README.md, assets) → Commit changes.
3. vercel.com → Continue with GitHub → Add New → Project → Import `surfcollective`.
4. Framework Preset: Other. No build command. Click Deploy.
5. Live at https://surfcollective.vercel.app (if the name is free). Every commit to GitHub redeploys automatically.
