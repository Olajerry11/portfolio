# Images Required for Your Portfolio

## Folder Location
All images go in: **`image_files/`** (create if it doesn't exist)

---

## Required Images

### 1. **showcase.jpg** (REQUIRED - Hero Background)
- **What it is:** Large background image for the hero/showcase section at top of homepage
- **Size:** 1600×900 pixels (or 1920×1080)
- **Format:** JPG or WebP
- **Where to download:**
  - Unsplash: https://unsplash.com (search: "technology workspace", "developer desk", "coding")
  - OR quick random: https://source.unsplash.com/1600x900/?technology,web
  - OR Pexels: https://www.pexels.com (search: "technology")
- **Folder:** `image_files/showcase.jpg`

---

### 2. **my-logo.png** (REQUIRED - Site Logo)
- **What it is:** Your personal logo shown in header (top left of every page)
- **Size:** 200×200 pixels (or larger)
- **Format:** PNG (with transparency) or SVG
- **Where to get:**
  - Design your own in Canva (free): https://www.canva.com
  - OR use a logo maker: https://looka.com or https://brandmark.io
  - OR use initials: "O" or "Olayiwola"
- **Folder:** `image_files/my-logo.png`
- **Note:** This is in your root already but should ideally be in `image_files/`

---

### 3. **logo_html.svg** (REQUIRED - HTML Icon)
- **What it is:** Icon for HTML5 service box
- **Size:** 80×80 – 120×120 pixels
- **Format:** SVG (scalable, best) or PNG
- **Where to download:**
  - Devicons (FREE SVG): https://raw.githubusercontent.com/devicons/devicon/master/icons/html5/html5-original.svg
  - OR Icons8: https://icons8.com/icons/set/html5
- **Folder:** `image_files/logo_html.svg`

---

### 4. **logo_css.svg** (REQUIRED - CSS Icon)
- **What it is:** Icon for CSS3 service box
- **Size:** 80×80 – 120×120 pixels
- **Format:** SVG or PNG
- **Where to download:**
  - Devicons (FREE SVG): https://raw.githubusercontent.com/devicons/devicon/master/icons/css3/css3-original.svg
  - OR Icons8: https://icons8.com/icons/set/css3
- **Folder:** `image_files/logo_css.svg`

---

### 5. **logo_js.svg** (REQUIRED - JavaScript Icon)
- **What it is:** Icon for JavaScript service box
- **Size:** 80×80 – 120×120 pixels
- **Format:** SVG or PNG
- **Where to download:**
  - Devicons (FREE SVG): https://raw.githubusercontent.com/devicons/devicon/master/icons/javascript/javascript-original.svg
  - OR Icons8: https://icons8.com/icons/set/javascript
- **Folder:** `image_files/logo_js.svg`

---

### 6. **logo_python.svg** (REQUIRED - Python Icon)
- **What it is:** Icon for Python service box
- **Size:** 80×80 – 120×120 pixels
- **Format:** SVG or PNG
- **Where to download:**
  - Devicons (FREE SVG): https://raw.githubusercontent.com/devicons/devicon/master/icons/python/python-original.svg
  - OR Icons8: https://icons8.com/icons/set/python
- **Folder:** `image_files/logo_python.svg`

---

### 7. **logo_cpp.svg** (REQUIRED - C++/Graphics Icon)
- **What it is:** Icon for Graphics Design / C++ service box
- **Size:** 80×80 – 120×120 pixels
- **Format:** SVG or PNG
- **Where to download:**
  - Devicons (FREE SVG): https://raw.githubusercontent.com/devicons/devicon/master/icons/cplusplus/cplusplus-original.svg
  - OR use a design/graphics icon: https://icons8.com/icons/set/design
- **Folder:** `image_files/logo_cpp.svg`

---

### 8. **profile.jpg** (OPTIONAL - About Page Photo)
- **What it is:** Your profile/headshot photo on About page
- **Size:** 400×400 pixels
- **Format:** JPG or WebP
- **Where to download:**
  - Unsplash: https://unsplash.com (search: "professional portrait", "headshot")
  - OR Pexels: https://www.pexels.com
  - OR use your own photo
- **Folder:** `image_files/profile.jpg`
- **Note:** Only needed if you want to add it to About page

---

## Quick Summary Table

| Filename | Type | Purpose | Folder |
|----------|------|---------|--------|
| showcase.jpg | Background | Hero/hero section | image_files/ |
| my-logo.png | Logo | Header logo | image_files/ |
| logo_html.svg | Icon | HTML5 box | image_files/ |
| logo_css.svg | Icon | CSS3 box | image_files/ |
| logo_js.svg | Icon | JavaScript box | image_files/ |
| logo_python.svg | Icon | Python box | image_files/ |
| logo_cpp.svg | Icon | C++/Graphics box | image_files/ |
| profile.jpg | Photo | About page (optional) | image_files/ |

---

## Download Instructions (PowerShell)

```powershell
# Navigate to project
cd "c:\Users\USER\OneDrive\Documents\My Portfolio"

# Create folder
New-Item -ItemType Directory -Path .\image_files -Force

# Download showcase background
Invoke-WebRequest "https://source.unsplash.com/1600x900/?technology,web" -OutFile .\image_files\showcase.jpg

# Download tech icons (SVG from Devicons)
Invoke-WebRequest "https://raw.githubusercontent.com/devicons/devicon/master/icons/html5/html5-original.svg" -OutFile .\image_files\logo_html.svg
Invoke-WebRequest "https://raw.githubusercontent.com/devicons/devicon/master/icons/css3/css3-original.svg" -OutFile .\image_files\logo_css.svg
Invoke-WebRequest "https://raw.githubusercontent.com/devicons/devicon/master/icons/javascript/javascript-original.svg" -OutFile .\image_files\logo_js.svg
Invoke-WebRequest "https://raw.githubusercontent.com/devicons/devicon/master/icons/python/python-original.svg" -OutFile .\image_files\logo_python.svg
Invoke-WebRequest "https://raw.githubusercontent.com/devicons/devicon/master/icons/cplusplus/cplusplus-original.svg" -OutFile .\image_files\logo_cpp.svg

# Optional: Download profile photo
Invoke-WebRequest "https://source.unsplash.com/400x400/?professional,portrait" -OutFile .\image_files\profile.jpg

# Verify downloads
dir .\image_files
```

---

## Next Steps

1. **Download all 7 REQUIRED images** using the PowerShell commands above
2. OR manually download them from the links provided and save to `image_files/` folder
3. For `my-logo.png` — create your own logo or use your initials
4. Once all images are in place, run `git add . && git commit -m "Add portfolio images"`
5. Then `git push origin main`

✅ **REQUIRED:** showcase.jpg, my-logo.png, logo_html.svg, logo_css.svg, logo_js.svg, logo_python.svg, logo_cpp.svg
⏳ **OPTIONAL:** profile.jpg (only if you want to add your photo to About page)
