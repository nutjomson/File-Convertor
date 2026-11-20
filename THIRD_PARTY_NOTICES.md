# Third-party notices

This repository vendors the following direct browser dependencies. The versions below are pinned by `.github/workflows/vendor-dependencies.yml`.

| Component | Version | License selected / declared | License text |
|---|---:|---|---|
| PDF.js (`pdfjs-dist`) | 2.16.105 | Apache-2.0 | [PDF.js LICENSE](THIRD_PARTY_LICENSES/pdfjs-dist/LICENSE) |
| pdf-lib | 1.17.1 | MIT | [pdf-lib LICENSE](THIRD_PARTY_LICENSES/pdf-lib/LICENSE.md) |
| jsPDF | 4.2.1 | MIT | [jsPDF LICENSE](THIRD_PARTY_LICENSES/jspdf/LICENSE) |
| JSZip | 3.10.1 | MIT option selected (upstream offers MIT or GPLv3) | [JSZip license terms and selected MIT text](THIRD_PARTY_LICENSES/jszip/LICENSE.markdown) |
| FileSaver.js | 2.0.5 | MIT | [FileSaver LICENSE](THIRD_PARTY_LICENSES/file-saver/LICENSE.md) |
| Cropper.js | 1.5.13 | MIT | [Cropper LICENSE](THIRD_PARTY_LICENSES/cropperjs/LICENSE) |
| SortableJS | 1.15.0 | MIT | [SortableJS LICENSE](THIRD_PARTY_LICENSES/sortablejs/LICENSE) |
| Tesseract.js | 5.1.1 | Apache-2.0 | [Tesseract.js LICENSE](THIRD_PARTY_LICENSES/tesseract.js/LICENSE) |
| Tesseract.js-core | 5.1.1 | Apache-2.0 for its own source; compiled WASM also bundles third-party components | [Core LICENSE](THIRD_PARTY_LICENSES/tesseract.js-core/LICENSE) |
| Tesseract OCR trained data (Thai/English) | tessdata 4.0.0 | Apache-2.0 | [tessdata LICENSE](THIRD_PARTY_LICENSES/tessdata/LICENSE) |

## Important scope and remaining license review

This is a direct-dependency notice, **not a complete Software Bill of Materials (SBOM) or legal opinion**.

In particular, the Tesseract.js-core README states that its compiled core is built from Tesseract and other third-party dependencies. The upstream project has also documented separate licenses for bundled components such as Leptonica, libwebp, giflib and zlib. The exact full component inventory and all required notices for the shipped 5.1.1 WASM binaries have not yet been independently verified against the exact npm tarball. See the [upstream core README](https://github.com/naptha/tesseract.js-core) and [upstream license discussion](https://github.com/naptha/tesseract.js-core/issues/44). Do not treat the Apache-2.0 file alone as proof that every object code component inside the WASM has been fully attributed.

The minified browser distributions may also bundle transitive code. A complete redistribution clearance requires reviewing the exact package tarballs, their embedded license banners, dependency metadata and applicable notices, not just the top-level package license.

## Upstream projects

- PDF.js: https://github.com/mozilla/pdf.js
- pdf-lib: https://github.com/Hopding/pdf-lib
- jsPDF: https://github.com/parallax/jsPDF
- JSZip: https://github.com/Stuk/jszip
- FileSaver.js: https://github.com/eligrey/FileSaver.js
- Cropper.js: https://github.com/fengyuanchen/cropperjs
- SortableJS: https://github.com/SortableJS/Sortable
- Tesseract.js: https://github.com/naptha/tesseract.js
- Tesseract.js-core: https://github.com/naptha/tesseract.js-core
- Tesseract OCR language data: https://github.com/tesseract-ocr/tessdata
