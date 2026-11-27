# Baseline Rally

A 2.5D tactical tennis arcade game built with vanilla JavaScript, HTML5 Canvas, and the Web Audio API. Shipped with no framework, no depnedencies, no build tools. All players will have to do is just open the index.html and play.

---

## Project Structure

baseline-rally/
    index.html
    style.css
    /js
        main.js
        physics.js
        ai.js
        audio.js

---

## How to Run

No server is required. Open the index.html file in any MODERN browser.
Chrome or Firefox is reccomended.

---

## Controls

**Note:** The controls were edited by AI because I had some keybinds which were duplicates.

Move - WASD or Arrow Keys
Sprint - Hold Shift (Drains stamina)
Flat Drive - Space or J
Topspin - K or Z
Slice - L or X
Aim Left - Hold A or Left Arrow during shot
Aim Right - Hold D / Right Arrow during shot
Pause - Escape

---

## Shot Types

Flat Drive - Low arc, high pace. Use for winners inside the baseline.
Topspin - High clearnace, dips sharply, kicks forward onbounce.
Slice - Floats low over the net, skids on landing, buys time.
Lob - High defensive arc to clear a net-rushing opponent.

---

## Difficulty Tiers

Rookie - 420ms reaction delay, 200 px/s movment
Club Player - 250ms reaction delay, 265 px/s movement
Tour Pro - 110ms reaction deloy, 330 px/s movement

---

## Match Formats

1-Set Sprint - First to 6 games wins.
Best-of-3 Sets - First to win 2 sets wins the match.
Endless Practice - No score tracking, rally indefinitely.

---

## Physics Notes

The ball tracks, x,y, and z coordinates. Gravity and spin affect the z-axis each frame. The 2.5D effect comes from offsetting the draw postion by ball.z and scaling the raidu with height. Net height is 28 units; balls crossing below z = 24 are dead.

---

## License

MIT