# Five & A+ Interactive Learning Site

Static GitHub Pages-ready version of the Five & A+ course learning site.

## What is included

- `25` courses
- `184` unit pages
- `847` lessons
- `6575` interactive questions
- Chunked loading: hub → course → unit
- Browser-saved progress using `localStorage`
- No build step required

## Folder structure

```text
.
├── index.html
├── 404.html
├── .nojekyll
├── README.md
├── manifest.json
├── site-manifest.json
├── assets/
│   ├── site.css
│   └── app.js
├── courses/
│   └── course overview pages
├── units/
│   └── individual unit pages
└── original_uploads/
    └── preserved original course HTML files
```

## How to upload to GitHub Pages

1. Create a new GitHub repository.
2. Upload the **contents of this folder** to the repo root. Do not upload the folder itself as a nested folder.
3. Commit the files.
4. Go to **Settings → Pages**.
5. Under **Build and deployment**, choose **Deploy from a branch**.
6. Select `main` and `/root`.
7. Save.
8. Open the Pages URL GitHub gives you.

## Local preview

You can open `index.html` directly in your browser. For the closest GitHub Pages behavior, run a simple local server:

```bash
python -m http.server 8000
```

Then open:

```text
http://localhost:8000
```

## Important

Progress is saved per browser using `localStorage`. If a student clears browser data or switches devices, their local progress will not carry over.
