# Third-party notices

The standalone `index.html` embeds jsQR 1.4.0 for decoding packaging QR codes.

- Project: https://github.com/cozmo/jsQR
- License: Apache-2.0. Full terms are in `LICENSE-jsQR.txt` and embedded in the HTML.
- The distribution was minified using Terser. No CDN request is required to load the decoder.

Online component-parameter lookups primarily use the LCSC public product parameter table via a dedicated API at https://component-parameters-exsheeper11.rubbishmaster11.chatgpt.site. The API validates C identifiers and only contacts a fixed LCSC product endpoint. It has no database and receives no photos, orders or inventory. Public parameter snapshots for four reported part identifiers are included as a fallback.

Fallback lookups use the public jlcsearch service, typed component tables and EasyEDA component cache: https://github.com/tscircuit/jlcsearch. Only the requested LCSC part number and public package/value filters are sent; packaging photos are decoded locally. Official missing values are not inferred from model numbers or voltage ranges. Existing browser inventory is retained.

LCSC packaging `pc`, `pm`, and `qty` field semantics were researched using https://github.com/theautomatist/scan2place. The label parser in this application was independently implemented.
