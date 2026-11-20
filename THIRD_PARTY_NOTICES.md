# Third-party notices

The application uses the following pinned browser libraries, now stored locally under `vendor/` rather than loaded from public CDNs at runtime.

| Component | Version | License |
|---|---:|---|
| PDF.js (`pdfjs-dist`) | 2.16.105 | Apache-2.0 |
| pdf-lib | 1.17.1 | MIT |
| jsPDF | 4.2.1 | MIT |
| JSZip | 3.10.1 | MIT (upstream package may list dual licensing; check package metadata) |
| FileSaver.js (`file-saver`) | 2.0.5 | MIT |
| Cropper.js | 1.5.13 | MIT |
| SortableJS | 1.15.0 | MIT |
| Tesseract.js | 5.1.1 | Apache-2.0 |
| Tesseract.js-core | 5.1.1 | Apache-2.0 |
| Tesseract OCR language data | tessdata 4.0.0 | See upstream tessdata repository/license terms |

The build workflow downloads the pinned npm packages and OCR language data, then commits the runtime files into `vendor/`. Available upstream license/NOTICE files copied from package distributions are in `THIRD_PARTY_LICENSES/`.

This is a direct-component inventory, not a complete Software Bill of Materials (SBOM). Some packages bundle or depend on transitive components. Before commercial redistribution, verify the complete dependency tree, all embedded notices, OCR trained-data terms, and the exact license texts for the shipped versions. Do not assume this file alone constitutes legal clearance.

Upstream projects:
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
