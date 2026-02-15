# Classlist Builder

> 🌐 **Live app:** https://wiggwigg.github.io/classlist/

Transform an Allocate/Excel student export into a structured class-list workbook in your browser, with optional photo tab generation from an Oracle Reports `.mhtml` photo report.

## ✨ What This App Does

- Builds a **master tab** with all students
- Creates **one class tab per class** (for example, `Tutorial 01`)
- Optionally creates a **photo tab per class** (for example, `Tutorial 01 Photos`)
- Sorts students by **Last name**, **First name**, then **Student ID**
- Adds internal links between tabs for fast navigation

## 🧩 Key Features

- **Flexible column mapping** for `Unique ID`, `Student Name`, `Student ID`, and optional `Student Email`
- **Weeks mode** (optional):
  - `Include Weeks` toggle
  - configurable total weeks, start date, and class-free week
  - week headers formatted as `01 - dd/mm`
  - class-free week highlighted in light grey
- **Master tab enhancements**:
  - `Class` column after `Student Email`
  - links from `Student ID` and `Class` to the exact student row in class tabs
  - week cells reference class-tab week cells
- **Class tab enhancements**:
  - title row (14pt, blue)
  - mailto links for populated student emails
  - week columns with thin borders and row borders
- **Photo report support (optional)**:
  - load a `.mhtml` / `.mht` photo report file
  - generates a second photo grid tab for each class with:
    - student photo
    - student name
    - student ID
  - if no photo report is selected, only class list tabs are created

## 📥 Inputs

1. **Excel source file** (`.xlsx` / `.xls`)  
2. **Photo report file** (`.mhtml` / `.mht`, optional)

## 📤 Output

The app downloads one `.xlsx` workbook containing:

- `Master` unit tab
- class list tabs (all first)
- photo tabs (after class tabs, only when a photo report is provided)

## 🚀 Run Locally

Open `index.html` in a browser.

## 🔒 Privacy

All processing runs in your browser session.  
No data is uploaded or stored by this app.

## 🛠 Deployment

GitHub Pages is configured with a workflow deploy.

- Push to `main` → Pages updates automatically
- Workflow file: `.github/workflows/pages.yml`
