# Meme Wars Template 🎨🔥

Welcome to **Meme Wars!**  
This repo is your team’s **starting point** for creating and sharing memes during the Get-Gitty Workshop.  

👉 When you fork this repo, it becomes your team’s website, published automatically with **GitHub Pages**.  
👉 That site will be shown live on the **Get-Gitty Event Page** alongside all other competing teams.  

---

## 🚀 Quick Start (3 steps)

1. **Use this template**  
   - Click the green **“Use this template”** button at the top of the repo.  
   - Select **“Create a new repository”**.  
   - Name it exactly as suggested by the registration system:  
     ```
     <team-slug>-meme-war
     ```
     Example: `git-happens-meme-war`

2. **Enable GitHub Pages**  
   - Go to your new repo: `https://github.com/<your-username>/<team-slug>-meme-war`  
   - Click **⚙️ Settings → Pages**  
   - Under **Build and deployment**:  
     - Source: **Deploy from a branch**  
     - Branch: `main` → Folder: `/ (root)`  
   - Save → wait 1–2 minutes → your live site will be here:  
     ```
     https://<your-username>.github.io/<team-slug>-meme-war/
     ```

3. **Add your memes**  
   - Create files inside the `memes/` folder (one per meme).  
   - Put images in `assets/images/`.  
   - Update `script.js` to include your new meme pages.  
   - Commit & push → your live site updates automatically.

---

## 📂 Folder Structure

meme-wars-template/
├── index.html # Entry point (rotates through your memes)
├── style.css # Shared styles
├── script.js # Rotator logic (edit MEMES list here)
├── README.md # This guide
├── memes/ # 👈 Add your meme HTML files here
│ ├── leader/
│ │ ├── 001-first-meme.html
│ │ └── images/ # personal images for leader
│ ├── alice/
│ │ └── 001-debugging.html
│ └── bob/
│ └── 001-deploy-friday.html
└── assets/ # Shared team assets
└── images/
└── team-logo.png


---

## ✨ Meme Naming Rules

To avoid overwriting each other’s files:

1. Make a personal folder under `/memes/` with **your GitHub handle** or short name.  
   Example: `memes/alice/`  

2. Name your meme HTML files like this:  
001-short-title.html
002-another-meme.html

- Number = order (three digits, so sorting works)  
- Title = short, lowercase, hyphen-separated  

3. Images go in your own `images/` subfolder:  
memes/alice/images/ship-it.png


4. Use **relative paths** for images:  
```html
<img src="./images/ship-it.png" alt="Ship it">

🖼 Example Meme File

memes/alice/001-deploy-friday.html:

<!doctype html>
<meta charset="utf-8">
<title>Deploy Friday</title>
<style>
  body {
    margin:0; display:grid; place-items:center; height:100vh;
    background:#0ea5e9; color:#fff; font:700 40px/1.2 system-ui;
  }
  .card {
    background:rgba(255,255,255,.12);
    padding:24px 32px; border-radius:16px;
    box-shadow:0 10px 30px rgba(0,0,0,.15);
  }
</style>
<div class="card">
  Deploying on Friday… what could go wrong? 😅
  <div><img src="./images/ship-it.png" alt="Ship it" style="max-width:320px;margin-top:12px"></div>
</div>

🔄 Update the Rotator

Open script.js and add your new meme paths to the MEMES array:
const MEMES = [
  "memes/leader/001-first-meme.html",
  "memes/alice/001-deploy-friday.html",
  "memes/bob/001-debugging.html"
];

✅ Only one person (the team leader) should update script.js to avoid conflicts. Everyone else just creates their own files.

👩‍💻 Git Workflow

Clone your fork:
git clone https://github.com/<your-username>/<team-slug>-meme-war.git
cd <team-slug>-meme-war

Create your meme:
mkdir -p memes/<your-handle>/images
nano memes/<your-handle>/001-my-meme.html

Commit & push:
git add memes/<your-handle>
git commit -m "feat(<your-handle>): add 001-my-meme"
git push

🌐 Live URL

Once pushed, your team’s memes are visible at:

👉 https://<your-username>.github.io/<team-slug>-meme-war/

This will automatically appear on the Event Page during the competition. 🎉

🏆 Tips

Keep memes goofy, short, and fun — it’s a workshop, not a final exam.

Inline CSS is fine in your meme pages (keeps them self-contained).

GIFs and PNGs work best for quick laughs.

Don’t upload huge files (>2MB) — GitHub Pages can get slow.
