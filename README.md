# MR MONJUR Document Service

A simple Bengali-language document photo utility website.

## Features
- Passport photo: AI background removal (requires internet) and selectable white, light blue, red, or light green background.
- Document A4: center-based crop using a selected aspect ratio.
- ID Card A4: center-based crop using a selected aspect ratio.
- Download processed image and print / save as PDF.

## Run locally
Open `index.html` in a modern browser. An internet connection is needed for the passport background-removal model, which is loaded from the IMG.LY package CDN.

## Publish with GitHub Pages
1. Create a new GitHub repository.
2. Upload **all files and folders** from this project.
3. Open **Settings → Pages**.
4. Under **Build and deployment**, choose **Deploy from a branch**.
5. Select branch `main` and folder `/ (root)`, then click **Save**.
6. Wait for GitHub Pages to publish the site. The public URL will appear in the Pages section.

## Important notes
- Passport background removal uses the browser-side `@imgly/background-removal` package from `esm.sh`; the first use downloads the model and may take time.
- The other tools currently perform a centered crop only. They do not remove or recolor the background.
- This is a client-side starter project, not a complete document-processing platform. It does not upload images to a server or store user files.
- Test carefully on different phones and browsers before sharing publicly. Do not promise official passport-photo compliance; confirm the required photo dimensions and background rules for the destination country.
