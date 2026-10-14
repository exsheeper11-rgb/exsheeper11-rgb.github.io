# Third-party notices

The standalone `index.html` embeds jsQR 1.4.0 for decoding packaging QR codes.

- Project: https://github.com/cozmo/jsQR
- License: Apache-2.0. Full terms are in `LICENSE-jsQR.txt` and embedded in the HTML.
- The distribution was minified using Terser. No CDN request is required to load the decoder.

Online component-parameter lookups use the public jlcsearch service and its EasyEDA component cache: https://github.com/tscircuit/jlcsearch. Only the requested LCSC part number is sent; packaging photos are decoded locally.

LCSC packaging `pc`, `pm`, and `qty` field semantics were researched using https://github.com/theautomatist/scan2place. The label parser in this application was independently implemented.
