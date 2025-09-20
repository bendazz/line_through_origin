# Line Through Origin (y = a x)

A single-file, front-end only web app to fit a least-squares regression line constrained through the origin: y = a x.

- Add points by clicking on the canvas or by entering x,y and clicking "Add point".
- Remove a point with right-click (removes the nearest point to the cursor).
- Fit is computed as a = Σ(x·y) / Σ(x²).
- Data persists in your browser via localStorage.
- Import/export CSV (header: `x,y`).

## Run

Just open `index.html` in a browser. Or serve locally for file API safety:

```
# Python 3
python3 -m http.server 8080
# Then open http://localhost:8080
```

## Notes

- If all x = 0, Σ(x²) = 0 and the slope is undefined.
- Auto-scale can be toggled; it includes the origin in the view so the constraint is visually clear.