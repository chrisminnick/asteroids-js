# Asteroids

Using only JavaScript, call NASA's Near Earth Object Web Services and create a visualization of a collection of asteroids for a specific date. We access size, speed, distance, and hazardousness from NASA to create each asteroid. Click on the asteroids to save Earth!

This software was designed for WatzThis? as an educational lab to explore JavaScript functions and API calls. This lab purposefully does not include any JavaScript libraries.

## Configure

1. Clone this repository.
2. Get a NASA API key from https://api.nasa.gov/index.html#apply-for-an-api-key.
3. In the project root, create `api-key.js` by copying `api-key.example`.
4. Edit `api-key.js` and set your real key:

```js
window.NASA_API_KEY = 'YOUR_REAL_NASA_KEY';
```

Notes:
- `api-key.js` is gitignored and should not be committed.
- If `api-key.js` is missing, empty, or the API request fails, the app automatically uses `sample-data.json`.

## Run

Run from the project root with a static file server (recommended):

```bash
npx serve .
```

Then open the local URL printed by `serve` (usually `http://localhost:3000`).

Alternative (Python):

```bash
python3 -m http.server 8000
```

Then open `http://localhost:8000`.

## Use The App

1. Enter a date in the form.
2. Submit to load asteroids for that date.
3. Click an asteroid to destroy it.
