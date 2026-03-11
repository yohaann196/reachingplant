# reaching plant

an interactive canvas thing. a plant grows toward your cursor. when it reaches you, it dies.

the reaching was the point.

---

## what it does

vines grow from the bottom of the screen and chase your cursor. each one blooms a small flower at its tip. when the tip gets close enough to touch where you are, it wilts - drooping, browning, dropping petals. then a new one grows.

fireflies drift around in the background. occasional lines of text appear at the bottom when something dies.

## how to run it

just open the html file in a browser.

```
open index.html
```

works on mobile too - touch to move the cursor position.

## what's inside

everything is drawn on a `<canvas>`. no libraries.

- `Vine` — the main growing stem. chases the mouse, spawns side tendrils, grows leaves, blooms, then wilts when it arrives
- `Tendril` — smaller offshoots from the vine
- `Particle` — handles spores, falling petals, and fireflies
- the background has stars, a moon, ground mist, and a soil strip at the bottom

the wilt physics droop the vine sideways (direction is randomized per vine) and curve it downward before it fades out.

## details

- pure canvas, no SVG, no images
- touch supported
- around 600 lines total
