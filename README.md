# Bernadette A. Divina — Personal Portfolio Web Application

A clean, responsive, single-page personal portfolio and academic profile web application designed with a **clean, flat yellow design system** (strictly no neon colors or glowing drop-shadows) and optimized for instant zero-config deployment on **Vercel** or local hosting on **XAMPP Apache**.

---

## 🎨 Design System
- **Light Mode:** Crisp, clean background (`#fcfcfc`), deep slate text, and warm elegant golden-yellow accents (`#eab308` / `#ca8a04`).
- **Dark Mode:** Matte slate-900 (`#0f172a`) and slate-800 (`#1e293b`) card surfaces with soft, readable warm yellow accents. **Strictly flat, clean, and professional** with no neon colors or drop-shadow glows.
- **Typography:** `Plus Jakarta Sans` for body copy and `Space Grotesk` for technical data badges and headings.
- **Resume Printing:** Includes a dedicated `@media print` stylesheet that automatically formats the page into an executive single/multi-page printable CV when clicking **"Print Resume"**.

---

## 📁 Project Structure

```
c:\xampp\htdocs\DivinaPort\
├── index.html                  # Core single-page web app with Tailwind CDN + dynamic data engine
├── vercel.json                 # Vercel deployment configuration with clean URLs & headers
├── profile.jpg                 # Bernadette A. Divina profile photo
├── certificate.png             # DICT Certificate of Participation
├── project-placeholder.jpg     # Minimalist placeholder graphic for upcoming projects
├── assets/
│   ├── profile.jpg
│   ├── certificates/
│   │   └── dict-startup-challenge.png
│   └── projects/
│       ├── sarak-overview.png
│       ├── sarak-streets.png
│       ├── sarak-darkmap.png
│       ├── sarak-about.png
│       └── sarak-detail.png
└── README.md
```

---

## ⚙️ Central Data Object (`portfolioData`)

All content is managed through a central JavaScript data object at the top of the `<script>` tag in [`index.html`](file:///c:/xampp/htdocs/DivinaPort/index.html):

```javascript
const portfolioData = {
  personalInfo: {
    name: "Bernadette A. Divina",
    email: "badetdivina2@gmail.com",
    phone: "09979377343",
    address: "Dugong, Bucay, Abra",
    githubUsername: "badetdivina2-tech",
    githubUrl: "https://github.com/badetdivina2-tech",
    facebookUrl: "https://www.facebook.com/badet.divina",
    bio: "Hello! I'm an IT student who enjoys exploring technology, learning new skills, and discovering how things work...",
    profileImage: "./profile.jpg"
  },
  education: [ ... ],
  skills: [ ... ],
  projects: [ ... ],
  certificates: [ ... ]
};
```

To update your skills, projects, or contact details, edit the `portfolioData` object in [`index.html`](file:///c:/xampp/htdocs/DivinaPort/index.html) and refresh the browser.

---

## 🚀 How to Deploy to Vercel (Instant & Free)

### Option 1: Via GitHub & Vercel Dashboard
1. Push this folder to a GitHub repository:
   ```bash
   git init
   git add .
   git commit -m "Initial commit - Bernadette Divina portfolio"
   git branch -M main
   git remote add origin https://github.com/badetdivina2-tech/portfolio.git
   git push -u origin main
   ```
2. Log in to [vercel.com](https://vercel.com).
3. Click **"Add New"** > **"Project"** and import the GitHub repository.
4. Leave all build settings default (Framework Preset: **Other**) and click **"Deploy"**.

### Option 2: Via Vercel CLI
```bash
npm i -g vercel
vercel
```

---

## 💻 Local Testing via XAMPP
Since this repository is located in `c:\xampp\htdocs\DivinaPort`, you can start Apache in the **XAMPP Control Panel** and open:
👉 **[http://localhost/DivinaPort/](http://localhost/DivinaPort/)**
