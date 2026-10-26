# For Bee: GitHub Pages edition

The exact rose-red, blush and gold website, including all real photos, chat screenshots, video, supplied song and WhatsApp response. No ChatGPT hosting dependency.

## Easiest setup, no code or build required
1. Extract the ZIP on your computer.
2. Create a GitHub repository named `for-bee` (or any name).
3. Upload the contents of this extracted folder to the repository root. index.html, assets and media must be at the root, not inside another folder. Do not upload the ZIP itself.
4. In Settings > Pages, choose Deploy from a branch. Choose main and /(root), then Save.
5. GitHub will show your live URL on the Pages settings screen when publishing completes.

This method works without uploading .github, .nojekyll or source. index.html, assets and media are all that is required. The included prebuilt assets use relative paths so repository names do not break images, music or scripts.

## Automatic deployment for future code changes
Upload the source folder and .github/workflows/deploy.yml too. In Settings > Pages choose GitHub Actions as Source instead of Deploy from a branch. Then open Actions > Deploy website to GitHub Pages > Run workflow. Future pushes to main rebuild and deploy automatically. If your file picker hides .github, create the file directly using GitHub Add file > Create new file and use .github/workflows/deploy.yml as its full filename, then copy the included workflow content.

Use ONE publishing method. The workflow rebuilds source into source/dist. Branch publishing uses the prebuilt root files. Changes to source require rebuilding when using branch publishing.

## Editing
All copy and interactions: source/src/main.tsx
Design: source/src/style.css
Media: source/public/media
Local commands: cd source, npm ci, npm run dev
Build: npm run build
To refresh the root static version, copy the CONTENTS of source/dist to the repository root, replacing index.html, assets and media.

Music begins after tapping “Okay, hear me out.” Controls allow pause and mute. The Yes dialog opens WhatsApp addressed to +16144969387 with the requested message. The visitor must press Send.

GitHub Pages normally publishes a publicly accessible site, including the personal photos, chats, song, and WhatsApp destination bundled with it. A public repository also exposes the source files.

## Verification
TypeScript and production build pass with relative paths. All media files are included. No GPT authentication or hosting files are included. GitHub deployment itself must be run in your repository.
