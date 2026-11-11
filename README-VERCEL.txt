# LearnPlay Kids — Vercel Deployment

This package contains the existing LearnPlay Kids website prepared for Vercel as a static site.

## Files
- `index.html` — the complete website (HTML, CSS and JavaScript).
- `vercel.json` — Vercel static deployment and response-header configuration.

## Deploy with Vercel (GitHub)
1. Extract this ZIP file.
2. Create a new GitHub repository and upload `index.html` and `vercel.json` to the repository root.
3. Sign in to https://vercel.com/ and choose **Add New → Project**.
4. Import the GitHub repository.
5. In the project configuration:
   - Framework Preset: **Other**
   - Root Directory: `./`
   - Build Command: leave empty / override disabled
   - Output Directory: `./`
   - Install Command: leave empty / override disabled
6. Select **Deploy**.

## Deploy with Vercel CLI
If you have Node.js and Vercel CLI installed, open a terminal in the extracted folder and run:

```bash
npx vercel
```

Follow the prompts. For production deployment, run:

```bash
npx vercel --prod
```

## Notes
- This is a static HTML application; no build step or server-side runtime is required.
- Existing browser-side features and local browser storage continue to run in visitors' browsers.
- Progress stored in browser local storage is device/browser-specific; it is not synchronized between users or devices.
