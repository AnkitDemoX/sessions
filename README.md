# Meeting Debriefing Reports

A professional HTML-based debriefing document template for post-meeting analysis and team feedback.

## 📁 Folder Structure

```
debriefing-reports/
├── README.md                          # This file
├── .gitignore                         # Git ignore rules
├── index.html                         # Main debriefing template
├── images/                            # Event photos and screenshots
│   ├── README.md                      # Image guidelines
│   └── [event photos go here]
└── debriefs/                          # Archive of past debriefing reports
    └── 2026-08-25_infinity-studio/    # Example: organized by date and topic
        ├── debriefing.html
        └── images/
```

## 🚀 Getting Started

### 1. Clone or Create Repository
```bash
git clone https://github.com/yourusername/debriefing-reports.git
cd debriefing-reports
```

### 2. Add Event Photos
- Place your meeting/event photos in the `images/` folder
- Supported formats: JPG, PNG, WebP
- Recommended image size: 1200x900px or larger
- File naming: `opening.jpg`, `demo.jpg`, `team.jpg`, etc.

### 3. Edit the Template
- Open `index.html` in a text editor
- Replace placeholder text `[...]` with your actual data
- Update image URLs in the gallery section to match your filenames
- Example: `images/opening.jpg`

### 4. Preview Locally
- Double-click `index.html` to open in browser, OR
- Use VS Code extension: Live Server
- Check responsiveness on mobile/tablet

### 5. Push to GitHub
```bash
git add .
git commit -m "Add debriefing report for [meeting-name]"
git push origin main
```

## 🏢 Adding Logos

### Pega Logo Setup (Top-Left):
1. Save Pega logo as `images/pega-logo.png` (preferably transparent background)
2. In `index.html`, find: `<img src="[pega-logo-url]" alt="Pega Logo">`
3. Replace with: `<img src="images/pega-logo.png" alt="Pega Logo">`
4. Logo will appear prominently at top-left with "Pega Demo X Organization" label
5. Recommended size: 150px width × 70px height (transparent PNG)

### Client Logo Setup (Top-Right):
1. Save client logo as `images/client-logo.png` (or .jpg)
2. In `index.html`, find: `<img src="[client-logo-url]" alt="Client Logo">`
3. Replace with: `<img src="images/client-logo.png" alt="Client Logo">`
4. Logo will appear in the top-left of the header (auto-sized to 60px height)

### Client Details:
- Client Name: Edit header `[Client Name]` field
- Organization: Edit metadata section
- Contact: Add client contact person email
- Business Context: Add why session was important for them

**Logo Best Practices:**
- Transparent background PNG (preferred)
- Max 150px width × 60px height
- File size: < 100KB
- Maintain client brand guidelines

## 🌐 Hosting on GitHub Pages

### Enable GitHub Pages:
1. Go to repository **Settings** → **Pages**
2. Select **Source**: `main` branch
3. Select folder: `/ (root)` or `/docs` (if using docs folder)
4. GitHub will generate URL: `https://yourusername.github.io/debriefing-reports/`

### Access Your Report:
- Main template: `https://yourusername.github.io/debriefing-reports/index.html`
- Archived reports: `https://yourusername.github.io/debriefing-reports/debriefs/2026-08-25_infinity-studio/debriefing.html`

## 📝 Workflow for Multiple Reports

Each meeting gets its own folder:

```
debriefs/
├── 2026-08-25_infinity-studio/
│   ├── debriefing.html
│   └── images/
├── 2026-09-10_ai-capabilities/
│   ├── debriefing.html
│   └── images/
└── 2026-09-20_team-workshop/
    ├── debriefing.html
    └── images/
```

Copy `index.html` and rename it, or keep one master template.

## 🎨 Customization

### Colors
Edit the color codes in the `<style>` section:
- Primary: `#667eea` (purple-blue)
- Secondary: `#764ba2` (darker purple)
- Success: `#28a745` (green)
- Warning: `#ffc107` (amber)

### Sections
Add/remove sections by duplicating and modifying HTML blocks with class `section`

### Logo/Header
Replace header text with your company logo or branding

## 📋 Template Sections

- Executive Summary (metadata)
- Session Overview
- Engagement Metrics
- Event Images Gallery
- What Went Well
- Delivery Observations
- Areas for Improvement
- Audience Feedback
- Action Items
- Lessons Learned
- Recommendations

## 💡 Tips

✅ **Do:**
- Keep image file sizes under 500KB each
- Use consistent folder naming (YYYY-MM-DD_meeting-name)
- Update the image captions for clarity
- Version control your reports for historical tracking

❌ **Don't:**
- Upload extremely large image files (will slow page load)
- Use spaces in filenames (use hyphens instead)
- Remove CSS styling unless you know what you're doing

## 🔍 Image Guidelines

- **Optimal size:** 1200x900px or 4:3 aspect ratio
- **Format:** JPG for photos, PNG for screenshots
- **Naming:** Use descriptive names (opening.jpg, demo.jpg)
- **Privacy:** Blur or redact sensitive information before uploading

## 📱 Responsive Design

The template works on:
- 📱 Mobile phones (320px+)
- 📱 Tablets (768px+)
- 🖥️ Desktops (1024px+)
- 🖨️ Print-friendly

## 🆘 Troubleshooting

**Images not showing?**
- Check file paths match exactly (case-sensitive on Linux)
- Use relative paths: `images/photo.jpg` not `/images/photo.jpg`

**Page not loading from GitHub Pages?**
- Wait 1-2 minutes after pushing changes
- Clear browser cache (Ctrl+Shift+Del)
- Check repository Settings → Pages is enabled

**Links broken?**
- Verify file paths and extensions (.html not .htm)
- Test locally first before pushing to GitHub

## 📄 License

Internal use only. Customize for your organization.

---

**Created by:** Ankit Sharma | Demo X Organization  
**Last Updated:** August 27, 2026
