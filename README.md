# File Convertor

A responsive, browser-based PDF and image utility. The application and its runtime dependencies are stored in this repository.

## Features

- PDF pages to images, with cropping
- Split and merge PDF files
- JPG/images to PDF
- PDF annotation / paint tools
- Thai and English OCR
- PDF watermarking
- Live crop and paste

## Run locally

Serve the repository root with a local static web server, then open the local URL. For example:

```bash
python -m http.server 8000
```

Open `http://localhost:8000`. Opening the HTML directly as a `file://` URL may prevent browser workers and OCR assets from loading.

## GitHub Pages

In the repository, open **Settings → Pages**, choose **Deploy from a branch**, select `main` and `/(root)`, then save. The app loads libraries, PDF workers, OCR worker/WASM and Thai/English trained data from the same origin under `vendor/`.

## Privacy and security

- The HTML references no external CDN scripts or stylesheets.
- The Content Security Policy restricts scripts, styles, workers and network connections to same-origin resources plus browser-local `blob:` / `data:` URLs where needed.
- PDF and image processing is performed in the browser. OCR language data and workers are served from this repository.
- The application source has been statically checked for external asset references and common direct network-upload APIs. This is **not** a full independent security audit, browser runtime Network-panel audit, or guarantee against browser extensions, compromised hosting, or future code changes.
- The GitHub repository is public. That exposes the application source and vendored libraries, **not the documents selected in your browser**. For highly confidential company files, prefer running a local copy on a trusted machine and test with the machine's network disconnected or blocked by company policy before production use.

## Third-party components

Pinned browser dependencies and OCR language data are stored under `vendor/`. Upstream license texts that were present in the npm packages are copied under `THIRD_PARTY_LICENSES/`. See [THIRD_PARTY_NOTICES.md](THIRD_PARTY_NOTICES.md). Review all licenses and notices against your organization's commercial-use policy before redistribution.
