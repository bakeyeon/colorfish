# Color Fish Test — What Color Fish are you?

A scroll-driven pixel-art landing page for **Color Fish Test**, the experimental platform behind the paper *The Grue Divide: When Cognitive Accuracy Doesn't Predict Affective Alignment* (Kai Hyeyeon Park).

Scroll to dive in: the camera sinks below the surface and the seven Color Fish swim in one by one, then the page flows into the FAQ.

- **Take the test:** https://color-vision-spark-en.lovable.app/
- **Data:** https://osf.io/xub35/
- **Platform source:** https://github.com/bakeyeon/colorfish_public

## Files

| Path | What |
| --- | --- |
| `index.html` | The whole page: scroll dive (canvas), FAQ loader, contact footer |
| `faq.json` | FAQ content. Edit this file to change the questions and answers |
| `assets/*.png` | Background and the seven fish sprites |

## Run locally

```bash
python -m http.server 8000
```

Then open http://localhost:8000. Opening `index.html` directly shows the dive, but the FAQ needs a server to read `faq.json`.

## Debug

In the browser console, `colorfishSeek(0.5)` jumps to any point of the story (0–1) without scrolling.
