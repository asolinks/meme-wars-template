# 🎨 Meme Wars Template 🔥

> **Welcome to Meme Wars!** Your team's ultimate battleground for creating and sharing epic memes during the Get-Gitty Workshop.

When you fork this repository, it magically transforms into your team's live website, automatically published with **GitHub Pages**. Your site will be showcased live on the **Get-Gitty Event Page** alongside all competing teams! 🚀

---

## 🚀 Quick Start Guide

### Step 1: Create Your Repository
1. Click the green **"Use this template"** button at the top of this repo
2. Select **"Create a new repository"**
3. Name it exactly as suggested by the registration system:
   ```
   <team-slug>-meme-war
   ```
   **Example:** `git-happens-meme-war`

### Step 2: Enable GitHub Pages
1. Navigate to your new repo: `https://github.com/<your-username>/<team-slug>-meme-war`
2. Click **⚙️ Settings** → **Pages**
3. Under **Build and deployment**:
   - **Source:** Deploy from a branch
   - **Branch:** `main`
   - **Folder:** `/ (root)`
4. Save and wait 1-2 minutes
5. Your live site will be available at:
   ```
   https://<your-username>.github.io/<team-slug>-meme-war/
   ```

### Step 3: Start Creating Memes
1. Create your meme files in the `memes/` folder
2. Add images to `assets/images/` or your personal image folder
3. Update `script.js` to include your new meme pages
4. Commit & push → your live site updates automatically! ✨

---

## 📂 Project Structure

```
meme-wars-template/
├── 📄 index.html              # Entry point (rotates through memes)
├── 🎨 style.css               # Shared team styles
├── ⚙️  script.js              # Meme rotator logic
├── 📖 README.md               # This guide
├── 📁 memes/                  # 👈 Your memes go here!
│   ├── 📁 leader/             # Team leader's memes
│   │   ├── 001-first-meme.html
│   │   ├── 002-git-commit.html
│   │   └── 📁 images/         # Leader's personal images
│   │       └── team-spirit.gif
│   ├── 📁 alice/              # Alice's meme collection
│   │   ├── 001-debugging.html
│   │   ├── 002-merge-conflict.html
│   │   └── 📁 images/         # Alice's images
│   │       ├── bug-hunt.png
│   │       └── success-kid.jpg
│   └── 📁 bob/                # Bob's memes
│       ├── 001-deploy-friday.html
│       └── 📁 images/         # Bob's images
│           └── ship-it.png
└── 📁 assets/                 # Shared team resources
    ├── 📁 images/             # Common team images
    │   ├── team-logo.png
    │   └── workshop-banner.jpg
    └── 📁 fonts/              # Custom fonts (optional)
```

---

## ✨ Meme Creation Rules

### 🏷️ Naming Convention
To keep things organized and avoid conflicts:

1. **Create your personal folder:**
   ```
   memes/<your-github-handle>/
   ```
   Example: `memes/alice/`

2. **Name your meme files:**
   ```
   001-short-descriptive-title.html
   002-another-awesome-meme.html
   003-weekend-coding.html
   ```
   - **Number:** 3-digit sequence (001, 002, etc.)
   - **Title:** lowercase, hyphen-separated, descriptive

3. **Organize your images:**
   ```
   memes/<your-handle>/images/your-image.png
   ```

4. **Use relative paths in your HTML:**
   ```html
   <img src="./images/your-image.png" alt="Descriptive alt text">
   ```

---

## 🎨 Example Meme File

Here's a sample meme file structure:

**File:** `memes/alice/001-deploy-friday.html`

```html
<!doctype html>
<html lang="en">
<head>
    <meta charset="utf-8">
    <meta name="viewport" content="width=device-width, initial-scale=1">
    <title>Deploy on Friday</title>
    <style>
        body {
            margin: 0;
            display: grid;
            place-items: center;
            height: 100vh;
            background: linear-gradient(135deg, #667eea 0%, #764ba2 100%);
            color: white;
            font: 700 2.5rem/1.2 'Comic Sans MS', system-ui;
            text-align: center;
        }
        .meme-card {
            background: rgba(255, 255, 255, 0.15);
            backdrop-filter: blur(10px);
            padding: 2rem;
            border-radius: 20px;
            box-shadow: 0 15px 35px rgba(0, 0, 0, 0.2);
            max-width: 500px;
        }
        .meme-image {
            max-width: 100%;
            height: auto;
            border-radius: 10px;
            margin: 1rem 0;
        }
    </style>
</head>
<body>
    <div class="meme-card">
        <h1>Deploying on Friday...</h1>
        <img src="./images/ship-it.png" alt="This is fine dog in burning room" class="meme-image">
        <p>What could possibly go wrong? 😅</p>
    </div>
</body>
</html>
```

---

## 🔄 Update the Rotator

After creating your memes, update the rotator in `script.js`:

```javascript
const MEMES = [
    "memes/leader/001-first-meme.html",
    "memes/leader/002-git-commit.html",
    "memes/alice/001-deploy-friday.html",
    "memes/alice/002-debugging.html",
    "memes/bob/001-merge-conflict.html"
];
```

> ⚠️ **Important:** Only the **team leader** should update `script.js` to avoid merge conflicts!

---

## 👩‍💻 Git Workflow

### Initial Setup
```bash
# Clone your team's repository
git clone https://github.com/<your-username>/<team-slug>-meme-war.git
cd <team-slug>-meme-war

# Create your personal workspace
mkdir -p memes/<your-handle>/images
```

### Creating a New Meme
```bash
# Create your meme file
nano memes/<your-handle>/001-my-awesome-meme.html

# Add your changes
git add memes/<your-handle>/
git commit -m "feat(<your-handle>): add awesome debugging meme"
git push origin main
```

### Best Practices
- **Commit messages:** Use format `feat(<your-handle>): description`
- **File sizes:** Keep images under 2MB for optimal loading
- **Testing:** Check your memes locally before pushing
- **Collaboration:** Communicate with teammates about shared assets

---

## 🌐 Live Deployment

Once you push your changes, your team's meme collection will be live at:

### 🎯 Your Team's URL
```
https://<your-username>.github.io/<team-slug>-meme-war/
```

This URL will automatically appear on the **Get-Gitty Event Page** during the competition! 🎉

---

## 🏆 Pro Tips for Meme Mastery

- ⚡ **Keep it snappy:** Best memes are quick, witty, and relatable
- 🎨 **Inline CSS is fine:** Keeps meme files self-contained and portable
- 🖼️ **Image formats:** GIFs and PNGs work best for web display
- 📱 **Mobile-friendly:** Test on different screen sizes
- 🚀 **Performance:** Optimize images and avoid heavy animations
- 😄 **Have fun:** Remember, it's about learning and laughing together!

---

## 🔧 Troubleshooting

### Common Issues
- **Site not updating?** Wait 2-3 minutes after pushing, GitHub Pages needs time
- **Images not loading?** Check your relative paths and file names
- **Memes not rotating?** Verify your paths in `script.js` match your file structure
- **Merge conflicts?** Stick to your personal folder and coordinate with team lead

### Getting Help
- Check the [GitHub Pages documentation](https://docs.github.com/en/pages)
- Ask your workshop facilitators
- Collaborate with your team members!

---

## 🎊 Ready to Meme?

Your team's meme empire awaits! Start creating, collaborating, and competing. May the best memes win! 🏅

**Happy Meme-ing!** 🎨✨

---

*Built with ❤️ for the Get-Gitty Workshop*# meme-wars-template
