# September Family Sports — customer journey mockups

Eight live touchpoints of the campaign, from the first Instagram Reel to the
follow-up message that brings the family back online. Scrolling scrubs a 30s
film behind the page; every phone screen is clickable.

## Put it online with GitHub Pages

1. Create a new repository on GitHub (public, no README).
2. Upload **everything in this folder**, keeping the folder structure:

   ```
   index.html
   support.js
   vendor/       react + react-dom
   nw/           photography
   assets/       QR codes
   uploads/      film-faststart.mp4  (20 MB)
   ```

3. Repo **Settings → Pages → Source: Deploy from a branch**, branch `main`,
   folder `/ (root)`. Save.
4. Wait about a minute. Your link is:

   `https://<your-username>.github.io/<repo-name>/`

Share that URL. No build step, no install.

## Things worth knowing

- **Keep the folder structure.** Paths are relative. Uploading only
  `index.html` gives a blank page.
- **`uploads/film-faststart.mp4` is required** — it is the background film the
  scroll drives. Its index sits at the front of the file so it seeks instantly;
  do not re-encode or re-export it, or scrolling will stall until the whole
  20 MB downloads.
- **GSAP loads from a CDN**, so viewers need to be online. Without it the
  journey still renders and stays clickable; it just doesn't animate.
- **Private repo?** GitHub Pages needs a paid plan for private repos. For a
  quick private share, Netlify Drop (drag this folder onto netlify.com/drop)
  gives an unlisted URL for free.
