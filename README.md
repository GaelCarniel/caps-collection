# 🍺 Cap Collection

A personal beer cap inventory — fast, static, no backend.

## Project structure

```
caps-collection/
├── index.html          
├── src/data/
│   └── caps.csv        
└── public/images/      
```

---

## Running locally

Because the site fetches `caps.csv` via `fetch()`, you need a local server

**Option A — Python (built-in):**
```bash
python3 -m http.server 8080
```

**Option B — VS Code:**
Install the Live Server extension → right-click `index.html` → Open with Live Server.

---

## Updating your inventory

Edit `src/data/caps.csv` — open it in Excel, Numbers, or any text editor:

```
Nom,Quantité,Type,Photo
Kronenbourg 1664,3,beer,0001.jpg
Coca-Cola,1,soda,
```

| Column | Description |
|---|---|
| **Nom** | Cap name |
| **Quantité** | How many physical caps you own |
| **Type** | One of: `beer`, `soda`, `cider` |
| **Photo** | Filename only (e.g. `0001.jpg`), leave empty for emoji placeholder |

Drop photos in `public/images/` with matching filenames, then commit and push.

---

## Deploying to GitHub Pages

1. Push this folder to a GitHub repo.
2. Go to **Settings → Pages**.
3. Source: **Deploy from a branch** → `main` → `/ (root)` → Save.
4. Site is live at `https://carnielgael.github.io/caps-collection/`

Updates: just push to `main` — rebuilds in ~30 seconds.

---

## Image tips

- Standardized Photos
- Name files: `name_beer.jpg`
- JPG, PNG, or WebP all work

---

