Run  : python collect_data.py

A webcam window will open with a control panel overlay.

### Controls

| Key     | Action                        |
|---------|-------------------------------|
| 0–6     | Select gesture class          |
| SPACE   | Toggle auto-capture ON/OFF    |
| S       | Save a single frame           |
| Q       | Quit and save                 |

### What To Do

1. Press a **number key (0–6)** to select a gesture class
2. Perform that gesture in front of the webcam
3. Press **SPACE** to start auto-capturing (images save automatically)
4. Hold the gesture steady for a few seconds
5. Press **SPACE** again to stop auto-capture
6. Switch to the next class and repeat
7. **Target: 200–500 images per class** (progress bars shown on screen)

### Gesture Reference

| Key | Gesture              | What To Do With Your Hand                     |
|-----|----------------------|-----------------------------------------------|
| 0   | Open Palm            | Spread all 5 fingers wide, palm facing camera |
| 1   | Index Point          | Only index finger extended, others curled      |
| 2   | Two Fingers Up       | Index + middle finger extended (peace sign)    |
| 3   | Fist                 | Close all fingers into a fist                 |
| 4   | Pinch                | Touch thumb tip and index fingertip together   |
| 5   | Three Fingers Up     | Index + middle + ring fingers extended         |
| 6   | Three Fingers Down   | Three fingers curled/pointing downward         |

### Gesture → Cursor Action Mapping

| # | Gesture | Cursor Action | Details |
|---|---------|---------------|---------|
| 0 | **Open Palm** ✋ | **Move cursor** | Cursor follows your index fingertip position |
| 1 | **Index Point** ☝️ | **Left click** | Triggers after 2 steady frames (debounce) |
| 2 | **Two Fingers Up** ✌️ | **Right click** | Same debounce as left click |
| 3 | **Fist** ✊ | **Neutral / Stop** | No action — pause cursor control |
| 4 | **Pinch** 🤏 | **Drag** | Holds left mouse button; move hand to drag |
| 5 | **Three Fingers Up** 🤟 | **Scroll up** | Scrolls up per trigger |
| 6 | **Three Fingers Down**🤙 | **Scroll down** | Scrolls down per trigger |