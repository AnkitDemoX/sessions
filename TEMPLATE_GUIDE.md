# 📋 Template System Guide

## Overview

Your project now includes a **Template Selector** with multiple professional templates and **header color customization** for client branding.

---

## 🎯 Quick Start

### Step 1: Open Template Selector
```
Open: index.html
```

### Step 2: Choose a Color Theme
The selector includes preset colors:
- **Pega Blue** (#0066CC) - Default
- **MUFG Red** (#dc3545) - For MUFG projects
- **Purple** (#667eea) - Modern look
- **Green** (#28a745) - Success/positive theme
- **Coral** (#ff6b6b) - Creative projects
- **Google Blue** (#1a73e8) - Tech-focused

Or use the **custom color picker** to enter your own hex color.

### Step 3: Select a Template
Choose from available templates:
1. **Case Study Template** - Project success stories and impact reports
2. **Debriefing Report Template** - Post-meeting analysis and feedback

### Step 4: Edit Template Content
Each template has placeholder text [like this] that you can replace with your actual content.

---

## 📊 Available Templates

### 1. Case Study Template (`case-study-template.html`)

**Use for:**
- ✅ Client success stories
- ✅ Project deliverables and impact
- ✅ Demonstration outcomes
- ✅ Business transformation stories
- ✅ Technical achievement showcase

**Key Sections:**
1. **OVERVIEW** - Business problem, project scope, solution, proof
2. **Key Metrics** - 6 metric boxes (person-days, timeline, performance, features, etc.)
3. **DELIVERY HIGHLIGHTS** - Environment, end-to-end proof, performance
4. **TEAM CONTRIBUTION** - Team members and their roles
5. **CLIENT IMPACT** - Engagement, broader impact, recognition
6. **CHALLENGES OVERCOME** - Obstacles and solutions
7. **EXECUTIVE TAKEAWAY** - Key summary statement

**Best For:**
- Project completion reports
- Customer-facing case studies
- Board presentations
- Leave-behind assets

**Example Use Case:** MUFG Agentic Share Sale project report

---

### 2. Debriefing Report Template (`debriefing-template.html`)

**Use for:**
- ✅ Post-meeting analysis
- ✅ Team retrospectives
- ✅ Detailed feedback collection
- ✅ Event debriefs
- ✅ Training/workshop reviews

**Key Sections:**
1. **Executive Summary** - Metadata and overview
2. **Session Overview**
3. **Engagement Metrics**
4. **Event Images Gallery**
5. **What Went Well**
6. **Delivery Observations**
7. **Areas for Improvement**
8. **Audience Feedback**
9. **Action Items**
10. **Lessons Learned**
11. **Recommendations**

**Best For:**
- Team meetings & workshops
- Internal retrospectives
- Training event documentation
- Detailed feedback capture

---

## 🎨 Color Customization

### How It Works

1. **Select a preset color** from the color palette in index.html
   - OR use the **custom color picker**
   - OR enter a **hex color code** (e.g., #FF5733)

2. Your color choice is **automatically saved** to your browser (localStorage)

3. When you open any template, it **automatically applies** the selected color to the header

### Supported Color Formats
- Hex codes: `#0066CC`, `#FF5733`
- RGB equivalents also work
- Use any web-safe or custom color

### Color Theme Application
The selected color is used for:
- Header background (main gradient)
- Primary accent color in templates
- Section highlights and borders
- Visual hierarchy elements

### Example: Using Customer Colors

**MUFG Example:**
- Color: #dc3545 (MUFG Red)
- Header will display in red with darker red gradient
- Client branding maintained throughout document

**Custom Client Example:**
- Color: #003366 (Navy)
- Header displays in custom navy with darker gradient
- Client identity reinforced on every page

---

## 📝 How to Use Templates

### Basic Workflow

```
1. Go to index.html
   ↓
2. Select header color for client branding
   ↓
3. Choose template (Case Study or Debriefing)
   ↓
4. Edit content ([bracketed text])
   ↓
5. Print to PDF or save as HTML
   ↓
6. Share with client/team
```

### Editing Templates

Each template has **placeholder text in [brackets]**:
```
[Project Title]
[Client Name]
[Your actual content here]
```

**To Edit:**
1. Open the template in your browser
2. Click the **✏️ Edit Mode** button (instructions provided)
3. Download the HTML file
4. Open in a text editor (VS Code, Notepad, etc.)
5. Replace [bracketed text] with your content
6. Save the file
7. Open in browser to preview

Or directly edit in the browser using developer tools (F12).

### Printing/PDF Export

Each template includes a **🖨️ Print / PDF** button:
1. Click the button
2. Print to PDF (recommended)
3. Save with meaningful filename: `MUFG_Agentic_Case_Study.pdf`

---

## 📁 File Structure

```
your-project/
├── index.html                    (NEW - Template selector)
├── case-study-template.html      (NEW - Case study template)
├── debriefing-template.html      (Existing - Debriefing template)
├── TEMPLATE_GUIDE.md             (This file)
├── README.md                      (Original documentation)
├── QUICK_START.md                (Original quick start)
├── .gitignore
└── images/
    ├── pega-logo.png
    ├── client-logo.png
    └── [event photos]
```

---

## 🔄 Workflow: Creating a Case Study

### Example: MUFG Agentic Share Sale

**Step 1: Open Selector**
```
Open index.html in browser
```

**Step 2: Choose MUFG Red**
```
Select "MUFG Red" (#dc3545) color option
(Color is now saved for next use)
```

**Step 3: Open Case Study Template**
```
Click "Open Template" button on Case Study card
→ case-study-template.html opens with red header
```

**Step 4: Edit Content**
```
Replace these sections:
- [Project Title] → "MUFG Agentic Share Sale Experience"
- [Client Name] → "MUFG"
- [Business Problem] → Describe the challenge...
- [Delivery Stats] → Fill in metrics (7 days, 5 team members, etc.)
- [Team Members] → Nishant Patnaik, Ramya Vellanki, etc.
- [Client Impact] → Success metrics and feedback
```

**Step 5: Add Logos**
```
Replace [pega-logo-url] with path to Pega logo
Replace [client-logo-url] with path to MUFG logo
```

**Step 6: Print to PDF**
```
Click "🖨️ Print / PDF" button
Select "Save as PDF"
Filename: MUFG_Agentic_Case_Study.pdf
```

**Step 7: Share**
```
Email PDF to stakeholders
Or host on GitHub Pages for interactive version
```

---

## 💡 Tips & Best Practices

### Color Selection Tips
- ✅ Use client's brand color for professional look
- ✅ Test color contrast for readability
- ✅ Save custom colors in notes for consistency
- ✅ Use same color across multiple templates

### Content Tips
- ✅ Keep metrics concise and impactful
- ✅ Use bullet points for readability
- ✅ Include specific numbers and percentages
- ✅ Write executive takeaway as powerful summary

### Image Guidelines
- 📸 Recommended size: 1200x900px
- 📸 Format: JPG for photos, PNG for screenshots
- 📸 File size: < 500KB each
- 📸 Path: Use relative paths like `images/photo.jpg`

### Branding Guidelines
- 🏢 Always include client logo (top-right)
- 🏢 Include Pega logo with organization name
- 🏢 Match client's color scheme
- 🏢 Use consistent fonts and spacing

---

## 🚀 Advanced Features

### LocalStorage Color Persistence
Your selected color is automatically saved and will:
- Persist across browser sessions
- Apply to all templates you open
- Sync across the same browser

To reset to default: Clear browser data or select "Pega Blue"

### Print-Friendly Design
All templates include:
- ✅ Print CSS optimizations
- ✅ Professional page breaks
- ✅ High-quality PDF output
- ✅ Responsive design for all devices

### Mobile Responsive
Templates work on:
- 📱 Mobile phones (320px+)
- 📱 Tablets (768px+)
- 🖥️ Desktops (1024px+)
- 🖨️ Print layouts

---

## ❓ FAQ

**Q: Can I use multiple colors in the same report?**
A: Yes, download the HTML and manually edit the CSS to customize individual sections.

**Q: Will my color choice affect the debriefing template too?**
A: Yes, the same color is applied to both templates for consistency.

**Q: How do I share templates with my team?**
A: Share the HTML files directly, or use GitHub Pages for online access.

**Q: Can I add more templates?**
A: Yes! Create new templates following the same structure, add them to index.html, and test.

**Q: How do I change the logo?**
A: Replace [pega-logo-url] and [client-logo-url] in the template with your image paths.

**Q: Is my color choice saved permanently?**
A: Yes, in your browser's localStorage. Clearing browser data will reset it.

---

## 📞 Support

**Common Issues:**

| Issue | Solution |
|-------|----------|
| Color not applying | Clear browser cache, reload index.html |
| Template not loading | Check file paths are correct |
| Images not showing | Use relative paths (images/photo.jpg) |
| Print looks bad | Use "Print" button, not browser print |
| Logo cut off | Resize logo image or adjust img max-width |

---

## 🎓 Learning Resources

- **View the MUFG PDF example:** [MUFG_Agentic_Share_Sale1.0.pdf]
- **Read original README:** README.md
- **Quick setup guide:** QUICK_START.md
- **View templates:** index.html

---

## ✅ Version History

**v1.0 - October 4, 2026**
- ✨ Added template selector (index.html)
- ✨ Added Case Study template
- ✨ Added header color customization
- ✨ Added color persistence (localStorage)
- ✨ Maintained Debriefing Report template
- 🗑️ Removed MUFGDemoBuild_Review.html from template options

---

**Created by:** Claude Haiku 4.5 | Demo X Organization  
**Last Updated:** October 4, 2026

For questions or improvements, contact your documentation team.
