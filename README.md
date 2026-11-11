# Segro Park Northampton | GitHub browser-upload edition v1.6

**GitHub web uploader limit:** 25 MiB per file. This edition has 7 model parts, each **at most 20 MiB**, so all individual files can be added in the GitHub browser upload UI. The downloadable labelled DWG is 8.4 MiB. **Do not upload the ZIP as one file**: extract it and upload its contents with the correct directory structure.

3. Commit the files. Then go to **Settings → Pages → Build and deployment → Deploy from a branch**, select `main` and `/(root)`, and Save. Wait for the published URL to appear.
4. Test the site and the Autodesk, DWG download and DroneDeploy buttons.

**Model payload:** 135,242,336 bytes; the 7 parts are byte-for-byte identical to the original GLB when concatenated. The actual browser viewer transparently loads all 7 and reconstructs the same 3D model. This is a presentation model, not an engineering measurement tool. The Autodesk Viewer share link is temporary (~30 days from 11 November 2026); the DWG download persists while the site is hosted.

**Local test:** In Terminal `cd` to the extracted directory and run `python3 -m http.server 8000 --bind 127.0.0.1`, then open `http://localhost:8000/`.

Branding update v1.7: SecurIT-only header; survey assets and links are unchanged.
