# East Tokyo Pocket Guide

A mobile map-first guide for an East Tokyo trip, published as a static GitHub Pages project with no build step, API key, or backend.

The map uses Leaflet with credential-free Esri label-free tiles and custom English district labels.

## Preview locally

From the project directory, run:

```sh
python3 -m http.server 8000
```

Open <http://localhost:8000/> in a browser. Do not open `index.html` directly with a `file://` URL if you want to test location access.

## Publish with GitHub Pages

1. Create a new public GitHub repository named `junkim100/tokyo-east-guide` without adding generated starter files.
2. Add this project as the repository contents and push the default branch to GitHub.
3. In the repository, open **Settings**, then **Pages**.
4. Under **Build and deployment**, choose **Deploy from a branch** as the source.
5. Select the default branch, choose the `/ (root)` folder, and save.
6. Wait for the Pages deployment to finish, then open <https://junkim100.github.io/tokyo-east-guide/>.

GitHub Pages serves the project over HTTPS. Browser geolocation requires HTTPS or localhost, asks for permission only after **Locate me** is tapped, and is unavailable when the page is opened directly from the filesystem.
