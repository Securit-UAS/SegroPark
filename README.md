# Segro Park Northampton | GitHub browser-upload edition v1.6

**GitHub web uploader limit:** 25 MiB per file. This edition has 7 model parts, each **at most 20 MiB**, so all individual files can be added in the GitHub browser upload UI. The downloadable labelled DWG is 8.4 MiB. **Do not upload the ZIP as one file**: extract it and upload its contents with the correct directory structure.

1. Obtain permission from McLaren / the project owner before public publishing: model and DWG will be public, and DroneDeploy share URL includes its access token.
2. Extract this ZIP locally. In your new GitHub repository, choose **Add file → Upload files**, then drag **the contents** of the extracted folder (`index.html`, `assets` folder, `downloads` folder and optionally `README.md`) into GitHub. Check that repository paths are `assets/segro.part01` ... `assets/segro.part07`, `assets/securit-logo.png`, `assets/mclaren-logo-white.png`, `downloads/Segro_Park_V2_Labelled.dwg` and `index.html` at the root. GitHub's browser may not preserve folder paths with every upload technique; check the paths before committing.
3. Commit the files. Then go to **Settings → Pages → Build and deployment → Deploy from a branch**, select `main` and `/(root)`, and Save. Wait for the published URL to appear.
4. Test the site and the Autodesk, DWG download and DroneDeploy buttons.

**Model payload:** 135,242,336 bytes; the 7 parts are byte-for-byte identical to the original GLB when concatenated. The actual browser viewer transparently loads all 7 and reconstructs the same 3D model. This is a presentation model, not an engineering measurement tool. The Autodesk Viewer share link is temporary (~30 days from 11 November 2026); the DWG download persists while the site is hosted.

**Local test:** In Terminal `cd` to the extracted directory and  run `python3 -m http.server 8000 --bind 127.0.0.1`, then open `http://localhost:8000/`.
