# Font Converter

Public GitHub Pages font converter with Facebook Blue UI.

## Supported font formats
- TTF
- OTF
- WOFF
- WOFF2

The converter reads these OpenType/TrueType font containers in the browser and can export to TTF, OTF, WOFF, or WOFF2 where the conversion is supported by FontTools.

## CSS Web Font Generator
After conversion the app automatically shows an `@font-face` CSS block with:
- font-family
- converted filename
- format()
- font-style
- font-weight
- font-display

There is also a **Copy CSS** button.

## Privacy
Fonts are processed locally in the browser using Pyodide + FontTools. The font file is not uploaded to your own server.

## Important limitation
“Any font format” cannot literally mean every font format ever created. Formats such as legacy EOT, SVG Font, bitmap fonts, and some proprietary formats require different conversion engines. This project covers the modern TTF/OTF/WOFF/WOFF2 family.

CFF/CFF2 outline conversion to TrueType outlines is not a lossless operation. The app therefore does not pretend that simply changing a file extension performs a safe outline conversion.

## GitHub Pages
Upload `index.html`, `README.md`, and `LICENSE` to a public repository, then enable GitHub Pages from the `main` branch and root folder.

## License
MIT
