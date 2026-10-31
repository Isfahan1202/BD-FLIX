# BD FLIX — Starter Website

A lightweight, mobile-friendly movie / series / anime catalogue made with plain HTML, CSS and JavaScript.

## Included
- Responsive minimal black-and-white design
- Search and category filters
- Title details popup
- HTML5 video player (only enabled when you add a video URL)
- No build step, package install, API key, or server required

## Run locally
Open `index.html` in a browser.

## Deploy from an Android phone with GitHub + Vercel
1. Sign in to GitHub and create a new **public** or **private** repository named `bd-flix`.
2. In the repository, choose **Add file → Upload files**.
3. Upload `index.html` from this ZIP (you can unzip it with your phone's Files app first).
4. Commit the upload.
5. Sign in to Vercel using GitHub.
6. Choose **Add New → Project**, import `bd-flix`.
7. Framework preset: **Other**. Build command: leave blank. Output directory: leave blank / default. Deploy.
8. Vercel will give you a `*.vercel.app` address.

If Vercel asks for a root directory, use `./` (the repository root). The `index.html` file must be at the root of the repository.

## Add your own catalogue entries
Open `index.html` in GitHub's file editor. Find the `const titles = [` section. Copy one entry and change its fields:

```js
{
  id: 9,
  title: "My Film",
  type: "Movie", // Movie, Series, or Anime
  year: 2026,
  genre: "Drama",
  description: "A short description.",
  colors: ["#334155", "#020617"],
  videoUrl: ""
}
```

For playback, set `videoUrl` to a direct MP4 URL that you own or are authorized to stream. Example format only:
`videoUrl: "https://your-authorized-host.example/video.mp4"`

Do not use scraped links, pirated streams, or video URLs that you do not have permission to use. Some hosts block playback on other websites. Prefer a legitimate video host that explicitly supports embedding or direct playback.

## Important
- This is a front-end starter, not a movie database or video hosting service.
- The sample titles are fictional placeholders.
- No copyrighted movie files are included.
- Do not upload large video files to Vercel. Host authorized media separately.
- Vercel Hobby is intended for personal, non-commercial use. Check current Vercel plan limits and terms before launch.
