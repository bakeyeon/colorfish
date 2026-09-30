# Color Fish Test — The Sea Where Light Disappears

A scroll-driven pixel-art landing page for **Color Fish Test**, the experimental platform behind the paper *The Grue Divide: When Cognitive Accuracy Doesn't Predict Affective Alignment* (Kai Hyeyeon Park).

Scroll to dive: the deeper you go, the more colors the water takes away. Red goes first, then orange, yellow and green. At the bottom, seven lights become the seven Color Fish.

- **Take the test:** https://color-vision-spark-en.lovable.app/
- **Data:** https://osf.io/xub35/
- **Platform source:** https://github.com/bakeyeon/colorfish_public

## Files

| Path | What |
| --- | --- |
| `index.html` | The whole page: scroll scene (canvas), FAQ loader, contact footer |
| `faq.json` | FAQ content. Edit this file to change the questions and answers |
| `assets/*.png` | Background and the seven fish sprites |
| `assets/sprites.js` | The same images as data URIs, used only when `index.html` is opened as a local file |

## Run locally

```bash
python -m http.server 8000
```

Then open http://localhost:8000. Opening `index.html` directly works for the dive, but the FAQ needs a server to read `faq.json`.

## Debug

In the browser console, `colorfishSeek(0.5)` jumps to any point of the story (0–1) without scrolling.
