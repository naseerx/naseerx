# README image sources

- `banner-light.html`, `banner-dark.html` → `../banner-light.png`, `../banner-dark.png` (1280×460, rendered at 2×)
- `daiary.html` → `../daiary.jpg` (1280×600, rendered at 2×, then converted to JPEG)

To change a number or a line of text, edit the HTML and re-render with headless Chrome:

    "/Applications/Google Chrome.app/Contents/MacOS/Google Chrome" --headless=new --hide-scrollbars \
      --force-device-scale-factor=2 --virtual-time-budget=8000 --user-data-dir=/tmp/readme-prof \
      --screenshot=$PWD/../banner-light.png --window-size=1280,460 file://$PWD/banner-light.html

Fonts (Literata, IBM Plex Mono) load from Google Fonts, so rendering needs a network connection.
