# File Convertor

A browser-based PDF and image utility. The responsive web app is served from `index.html`.

## Features

- PDF pages to images, with cropping
- Split and merge PDF files
- JPG/images to PDF
- PDF annotation / paint tools
- Thai and English OCR
- PDF watermarking
- Live crop and paste

## Run locally

Open `index.html` in a modern browser, or serve this repository with a static web server.

## GitHub Pages

In the repository, open **Settings → Pages**, choose **Deploy from a branch**, select `main` and `/(root)`, then save.

## Privacy and security status

The app is designed to process selected documents in the browser. A static source review did not find direct document-upload calls in the app code. However, this repository version still loads third-party JavaScript libraries and OCR resources from external CDNs / hosts.

**Do not use this hosted version for confidential company documents until the external dependencies (including OCR worker, WASM and language data) have been self-hosted and runtime network testing has confirmed that document contents are not transmitted to third parties.** Browser/CDN requests can still expose ordinary connection metadata such as IP address.

This repository has not yet undergone a full runtime security audit or a complete transitive dependency / license audit.

## Third-party libraries

See [THIRD_PARTY_NOTICES.md](THIRD_PARTY_NOTICES.md) for the direct library list and license identifiers.
