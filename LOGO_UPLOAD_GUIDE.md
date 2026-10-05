# 📁 Logo Upload Feature Guide

**Updated:** October 4, 2026  
**Version:** 2.0

---

## 🎯 What Changed

### ❌ Removed
- Color tile picker from template selector
- Color customization interface
- Color persistence system

### ✅ Added
- **Logo Upload** in both templates (Case Study & Debriefing)
- Click-to-upload logo areas in headers
- File input for easy logo management
- Placeholder graphics for empty logo slots

---

## 📸 How to Upload Logos

### Method 1: Click on Logo Area (Easiest)
1. Open any template (case-study or debriefing)
2. Click directly on the logo area in the header (it says "📁 Upload")
3. Select your logo file
4. Logo displays immediately

### Method 2: Use Upload Section
1. Open any template
2. See the "Upload Client Logos" section at the top
3. Click on the file input fields
4. Select Pega logo and Client logo
5. Logos update in real-time

### Method 3: File Input Fields
Both templates have dedicated file input fields:
- `pegaLogoInput` - Pega/Organization logo
- `clientLogoInput` - Client logo

---

## 📋 Template Changes

### **Case Study Template**
**File:** `case-study-template.html`

**Logo Upload Features:**
- ✅ Click on Pega logo area to upload
- ✅ Click on Client logo area to upload
- ✅ Dedicated upload section with instructions
- ✅ Recommended sizes: Pega 150×60px, Client 130×50px
- ✅ "Manage Logos" button to show/hide upload section

**New Elements:**
```html
<div class="logo-container" onclick="document.getElementById('pegaLogoInput').click()">
    <div class="logo-placeholder">📁 Upload Logo</div>
</div>

<input type="file" id="pegaLogoInput" accept="image/*" onchange="uploadPegaLogo(event)">
```

---

### **Debriefing Report Template**
**File:** `debriefing-template.html`

**Logo Upload Features:**
- ✅ Click on Pega logo area to upload
- ✅ Click on Client logo area to upload
- ✅ Visible upload section at page top
- ✅ Recommended sizes: Pega 180×70px, Client 150×60px
- ✅ Quick "Done" button to close upload section

**New Elements:**
```html
<div class="pega-logo-container" id="pegaLogoContainer" onclick="document.getElementById('pegaLogoInput').click()">
    <div class="pega-logo-placeholder">📁 Upload</div>
</div>

<input type="file" id="pegaLogoInput" accept="image/*" onchange="uploadPegaLogo(event)">
```

---

## 🔧 JavaScript Functions Added

Both templates now include these functions:

```javascript
// Upload Pega/Organization Logo
function uploadPegaLogo(event) {
    const file = event.target.files[0];
    if (file) {
        const reader = new FileReader();
        reader.onload = function(e) {
            const container = document.getElementById('pegaLogoContainer');
            container.innerHTML = `<img src="${e.target.result}" alt="Pega Logo">`;
        };
        reader.readAsDataURL(file);
    }
}

// Upload Client Logo
function uploadClientLogo(event) {
    const file = event.target.files[0];
    if (file) {
        const reader = new FileReader();
        reader.onload = function(e) {
            const container = document.getElementById('clientLogoContainer');
            container.innerHTML = `<img src="${e.target.result}" alt="Client Logo">`;
        };
        reader.readAsDataURL(file);
    }
}

// Toggle Upload Section
function toggleUploadSection() {
    const section = document.getElementById('logoUploadSection');
    section.classList.toggle('show');
}
```

---

## 📐 Recommended Logo Sizes

### Case Study Template
| Logo | Width | Height | Format |
|------|-------|--------|--------|
| Pega/Organization | 150px | 60px | PNG (transparent) or JPG |
| Client | 130px | 50px | PNG (transparent) or JPG |

### Debriefing Report Template
| Logo | Width | Height | Format |
|------|-------|--------|--------|
| Pega/Organization | 180px | 70px | PNG (transparent) or JPG |
| Client | 150px | 60px | PNG (transparent) or JPG |

---

## 🎨 How Logos Persist

**Browser Storage:**
- Logos are stored as **Data URLs** (base64 encoded) in memory
- They persist **during the session** (while browser tab is open)
- **They do NOT save** after closing the template

**Best Practice:**
1. Upload logos to template
2. Add your content
3. Click "🖨️ Print / PDF" immediately
4. Save the PDF (logos are embedded)

Or:

1. Edit template HTML to embed logo paths directly
2. Save the modified template
3. Open template later with permanent logo references

---

## ✨ Key Features

### Case Study Template
- ✅ Professional header with clickable logo areas
- ✅ Upload instructions section (collapsible)
- ✅ Real-time logo preview
- ✅ "Manage Logos" button to show/hide upload section
- ✅ Smooth transitions and hover effects

### Debriefing Report Template
- ✅ Professional header with clickable logo areas
- ✅ Visible upload section at page top
- ✅ Real-time logo preview
- ✅ "Done" button to collapse upload section
- ✅ Hover effects on logo areas

---

## 🚀 Usage Workflow

### Quick Start (2 minutes)

```
1. Open index.html
   ↓
2. Choose template (Case Study or Debriefing)
   ↓
3. Click on logo area or use upload section
   ↓
4. Select Pega logo file
   ↓
5. Click on client logo area
   ↓
6. Select Client logo file
   ↓
7. Logos now display in header
   ↓
8. Edit content
   ↓
9. Click "🖨️ Print / PDF"
   ↓
10. Save PDF
```

---

## 📝 Common Use Cases

### MUFG Case Study
1. Open `case-study-template.html`
2. Click Pega logo → Upload `pega-logo.png`
3. Click Client logo → Upload `MUFG_logo.png`
4. Fill in case study content
5. Print to PDF as `MUFG_Agentic_Case_Study.pdf`

### Internal Meeting Debrief
1. Open `debriefing-template.html`
2. Click Pega logo → Upload `pega-logo.png`
3. Click Client logo → Upload `client-logo.png` (optional)
4. Add meeting details and feedback
5. Print to PDF as `Meeting_Debrief_Date.pdf`

---

## 🔒 Security Notes

- ✅ Files are processed **locally** in your browser
- ✅ **No data sent** to any server
- ✅ Logos stored as **Data URLs** (base64 in memory)
- ✅ Safe to customize with client information

---

## 🐛 Troubleshooting

| Issue | Solution |
|-------|----------|
| Logo not showing | Ensure file is a valid image (JPG, PNG, etc.) |
| Logo upload section not visible | Click "📁 Manage Logos" button to show it |
| Logo disappears after refresh | Logos don't persist; save to PDF before closing |
| Logo looks pixelated | Use higher resolution image (recommended: 300dpi) |
| Logo not centered | Try PNG format with transparent background |

---

## 📋 Comparison: Before vs. After

### Before (v1.0)
- ❌ Color picker interface
- ❌ Placeholder image paths `[pega-logo-url]`
- ❌ Manual file path editing required
- ❌ Color persistence system
- ✅ 6 preset colors available

### After (v2.0)
- ✅ Logo upload interface
- ✅ Click-to-upload logo areas
- ✅ Real-time logo preview
- ✅ No file path editing needed
- ✅ Drag-and-drop ready (future enhancement)
- ❌ Color picker removed

---

## 🎯 Next Steps

### To Use Templates Now:
1. Open `index.html` to see template selector
2. Choose Case Study or Debriefing template
3. Upload your Pega and client logos
4. Edit content
5. Print to PDF

### To Make Logos Permanent:
Edit the template HTML directly:
```html
<!-- Replace this: -->
<input type="file" id="pegaLogoInput" ...>

<!-- With this: -->
<img src="images/pega-logo.png" alt="Pega Logo">
```

Then save the template file.

---

**Version:** 2.0 with Logo Upload  
**Updated:** October 4, 2026  
**Status:** Ready for production use
