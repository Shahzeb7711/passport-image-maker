# Passport Photo Maker

Browser-only passport photo tool. No server, no API keys.

## Run
- Locally: serve the folder (e.g. `python3 -m http.server`) and open http://localhost:8000
- Deploy: upload the folder as-is to Cloudflare Pages / any static host.

Opening index.html directly via file:// also works in most browsers.

## Contents
- index.html: the app; face detection, landmark and selfie-segmentation models are embedded inside it.
- vendor/face-api.js: @vladmandic/face-api 1.7.15 (bundles TensorFlow.js)
- vendor/jspdf.umd.min.js: jsPDF 2.5.1

## Notes
- Sizes: 35x45 mm, 51x51 mm (2x2 in), 25x35 mm. Papers: 4x6 in (8 photos), A4 (30 photos).
- Print the PDF at "Actual size" / 100% to get exact dimensions.
