# Reachy Mini Assembly Guide

Lena Hall's interactive 3D assembly guide, prepared as the product example for the AssemblyFlow demo with Pazi.

## Run locally

Serve this directory with any static web server. For example:

```sh
python3 -m http.server 8000
```

Open http://localhost:8000. No package installation, build step, API key, backend, or network asset download is required by this version.

## Deploy

The static document root is this repository's root. Deploy `index.html` and all three `reachy-assets-*.js` files together in the same directory. The script paths are relative, so the app can also be served from a `/guide/` directory on a landing-page site.

For the Pazi demo, have Pazi read this repository and deploy the real app through its verified hosting workflow. Record the source commit, deployment result, and public URL. A repository upload is not a deployment.

## Source packaging

The supplied `Reachy-Mini-Assembly.html` was 29,900,286 bytes, exceeding GitHub's browser upload limit for a single file. Its embedded asset map has been moved into three sequential local JavaScript files. All 96 embedded assets are preserved exactly, and the remaining application HTML and JavaScript are unchanged. The original supplied file remains untouched outside this repository.

`SOURCE.json` records the original file hash and hashes of the packaged app files.

## Attribution and publication status

The app retains its existing attribution and bundled license notices, accessible through its credits. It uses Pollen Robotics' Reachy Mini meshes and assembly-guide diagrams. This is an independent demonstration; no Pollen endorsement is claimed.

The source is being staged privately. The applicable redistribution terms for the bundled hardware assets and diagrams are still to be confirmed before public deployment. Existing attribution text is preserved from the supplied app and should not be treated as a completed rights review. This repository does not add a blanket license over third-party material.
