# 📄 How to Update Your CV PDF

**If you want to upload a new CV PDF file:**

## Steps:

### 1. Add your new PDF file
- Place your new CV PDF in the `assets/pdf/` folder
- **Recommended naming**: `Yukun-Ma-CV-v5.pdf` (increment the version number)

### 2. Update the CV page link
- Open the file: `_pages/cv.md`
- Find the line: `cv_pdf: Yukun-Ma-CV-v4.pdf`
- Change it to: `cv_pdf: Yukun-Ma-CV-v5.pdf` (or your new filename)
- **Save the file**

### 3. Optional - Clean up old files
- You can delete old CV versions from `assets/pdf/` folder if desired
- Keep at least the current version referenced in `cv.md`

## Example
If your new CV is named `Yukun-Ma-CV-v5.pdf`, your `_pages/cv.md` should look like:
```
cv_pdf: Yukun-Ma-CV-v5.pdf
```

---
[← Back to Main SOP](../SOP.md)
