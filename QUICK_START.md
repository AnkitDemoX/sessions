# 🚀 Quick Start Guide

Get your debriefing report live in 5 minutes.

## Step 1: Create GitHub Repository
```bash
# Create new repo on GitHub called "debriefing-reports"
# Clone to your computer
git clone https://github.com/yourusername/debriefing-reports.git
cd debriefing-reports
```

## Step 2: Copy This Folder Structure
```
debriefing-reports/
├── README.md                    (copy provided README)
├── .gitignore                   (copy provided .gitignore)
├── index.html                   (copy debriefing-template.html, rename to index.html)
└── images/                      (create this folder)
    └── [your event photos here]
```

## Step 3: Add Your Event Photos
```bash
# Copy your photos to the images/ folder
cp your-photos/* images/
```

## Step 4: Add Logos

**Pega Logo (Top-Left):**
```bash
cp pega-logo.png images/
```
In `index.html`, find and replace:
```html
<img src="[pega-logo-url]" alt="Pega Logo">
```
With:
```html
<img src="images/pega-logo.png" alt="Pega Logo">
```

**Client Logo (Top-Right):**
```bash
cp client-logo.png images/
```
In `index.html`, replace:
```html
<img src="images/TNB_logo.jpg" alt="Client Logo">
```
With:
```html
<img src="images/client-logo.png" alt="Client Logo">
```

## Step 5: Edit index.html
Open `index.html` in your text editor and replace:

| Find | Replace With |
|------|---------------|
| `[Client Name]` | Acme Corporation |
| `[Client Organization Name]` | Acme Corporation |
| `[Date]` | August 25, 2026 |
| `[Presentation title]` | Your actual title |
| `[image-url-1.jpg]` | `images/opening.jpg` |
| `[image-url-2.jpg]` | `images/presenter.jpg` |
| `[...]` | Your actual data |

## Step 6: Push to GitHub
```bash
git add .
git commit -m "Initial debriefing report setup"
git push origin main
```

## Step 7: Enable GitHub Pages
1. Go to GitHub repo → Settings
2. Scroll to "Pages"
3. Select "main" branch → "/" (root)
4. Click Save
5. Wait 1-2 minutes

Your site will be live at:
```
https://yourusername.github.io/debriefing-reports/
```

## 📝 Next Time

For future meetings, just:
1. Copy `index.html` to `debriefs/[date]-[topic]/debriefing.html`
2. Create `debriefs/[date]-[topic]/images/` folder
3. Add photos
4. Edit content
5. `git add . && git commit -m "..." && git push`

Done! 🎉

## 🆘 Common Issues

| Problem | Solution |
|---------|----------|
| Images not showing | Check file path is exact match (case-sensitive) |
| GitHub Pages not working | Wait 2 min, clear cache, check Settings |
| HTML won't open | Double-click index.html or use Live Server |
| Commit failed | Make sure you're in repo folder |

## 📚 Full Documentation

See `README.md` for complete details.
