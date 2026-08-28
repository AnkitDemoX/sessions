# Images Folder Guide

This folder stores event photos and screenshots for the debriefing reports.

## 📸 Naming Convention

Use descriptive, lowercase names with hyphens:
```
opening.jpg              # Opening remarks/intro
presenter.jpg            # Presenter on screen
team-photo.jpg          # Team group photo
demo-walkthrough.jpg    # Demo or screen share
audience.jpg            # Audience engagement
qa-session.jpg          # Q&A session
screen-capture-1.jpg    # Additional screenshots
```

## 🖼️ Image Specifications

- **Format:** JPG (photos) or PNG (screenshots)
- **Dimensions:** 1200x900px minimum (4:3 aspect ratio recommended)
- **File Size:** 100-500KB per image
- **Quality:** High quality, well-lit, clear visibility

## 📋 Folder Structure for Multiple Events

```
images/
├── 2026-08-25-infinity-studio/
│   ├── opening.jpg
│   ├── presenter.jpg
│   ├── demo.jpg
│   └── team-photo.jpg
├── 2026-09-10-capabilities/
│   ├── opening.jpg
│   ├── demo.jpg
│   └── audience.jpg
```

Then reference in HTML as: `images/2026-08-25-infinity-studio/opening.jpg`

## ✅ Checklist Before Uploading

- [ ] Images are clear and well-focused
- [ ] File size is optimized (< 500KB)
- [ ] No sensitive/confidential information visible
- [ ] Filename is descriptive and lowercase
- [ ] Privacy/faces are handled appropriately
- [ ] Image paths in HTML match exactly

## 🔒 Privacy & Security

- Blur or redact employee names/emails if visible
- Remove screen content with sensitive data
- Ask attendees for permission before using their photos
- Review for company logos/confidential info

## 🚀 Adding Images to Your Debriefing

In the HTML gallery section, update:
```html
<div class="gallery-item">
    <img src="images/your-image.jpg" alt="Description">
    <div class="gallery-item-caption">Image Caption</div>
</div>
```

## 💾 GitHub Best Practices

```bash
# Add images to git
git add images/
git commit -m "Add images for August 25 meeting"
git push origin main
```

Images will be served directly from your GitHub repository.

---

**Tips:** Keep images organized by date/event for easy management and quick access.
