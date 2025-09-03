# 🎮 Get Gitty Meme Wars - Template Repository

Welcome to the **Get Gitty Meme Wars!**  
This is your starter template for creating and submitting your hilarious meme.  
This guide will walk you through the entire process, from forking this repo to seeing your meme live on the competition website.

---

## 🚀 Quick Start Guide

### 1. Fork This Template
You must do this first! Click the **"Use this template"** button at the top of this page to create your own copy under your GitHub account.

**Important:** When asked for a Repository name, you **MUST** name it exactly as provided during your team registration.  
It will look like this:

```
<your-team-name>-meme-war
```

**Example:** If your team name is *"The Git Gurus"*, your repo must be named:

```
the-git-gurus-meme-war
```

---

### 2. Clone Your New Repository
Clone your newly forked repo to your local machine to start working on it.

```bash
# Replace YOUR-USERNAME and YOUR-REPO-NAME with your details
git clone https://github.com/YOUR-USERNAME/YOUR-REPO-NAME.git
cd YOUR-REPO-NAME
```

---

### 3. Create Your Meme Masterpiece!
Now for the fun part. Edit the files in this template to create your meme:

- **index.html** → Your main meme page. Add your HTML, CSS, and any JavaScript here.  
- **styles.css** → Add your custom styles here to make your meme look awesome.  
- **/assets** folder → Place any images, GIFs, or other media you want to use in here.  

✨ Be creative! Use any web technology you like. The only rule is that it must all be contained within your forked repository.

---

### 4. Push Your Code to GitHub
Once you're happy with your meme, it's time to send it to GitHub.

```bash
# Add all your changed files to the staging area
git add .

# Commit your changes with a descriptive message
git commit -m "Created our amazing meme! 🚀"

# Push your code to GitHub
git push origin main
```

---

### 5. Enable GitHub Pages
This is the **most important step!** It makes your meme visible on the live web.

1. Go to the **Settings** tab of your GitHub repository.  
2. On the left sidebar, click **Pages**.  
3. Under **Build and deployment**, set the **Source** to *Deploy from a branch*.  
4. Set the **Branch** to `main` and the folder to `/ (root)`.  
5. Click **Save**.  

Your meme will now be live at:

```
https://YOUR-USERNAME.github.io/YOUR-REPO-NAME/
```

⚠️ It can take a minute or two for your site to become available after you enable Pages.

---

### 6. You're Done! 🎉
The competition website will automatically detect your pushed meme within a few minutes.  
Once it does, your team's card will change from *"Meme Loading..."* to displaying your live creation!

👉 Go to the **main competition website** to see your meme and start collecting votes!

---

## 🏆 How Voting Works
- Your meme will appear on the **main competition website** in your team's card.  
- Anyone can vote for their favorite memes by clicking the **"Vote 👍"** button.  
- Voting is limited to **one vote per person**.  
- The leaderboard on the website updates in real-time.  

---

## 🛠️ Technical Details & Tips

### Project Structure
```
.
├── index.html      # The main page of your meme website
├── styles.css      # Your custom styles
├── script.js       # Your custom JavaScript (optional)
└── assets/         # Folder for your images and other media
    └── my-meme.jpg
```

### Need Inspiration?
- **Classic Image Meme:** Add an image to `index.html` and a funny caption.  
- **Animated CSS Meme:** Use CSS animations to make elements move or change.  
- **Interactive Meme:** Use JavaScript to create a meme that changes when you click or hover.  
- **Video Meme:** Embed a video file from your assets folder.  

### Getting Help
- ask your workshop facilitators!  

---

## ❓ Frequently Asked Questions

**Q: My meme isn't showing up on the website. What do I do?**  
- Double-check your repo name. It must be **exactly** as provided during registration.  
- Did you enable GitHub Pages? Go to **Settings → Pages** to confirm.  
- Did you push your code? You need to `git push` after making changes.  
- Wait a few minutes. The system checks for new memes every ~2 minutes.  

---

**Q: Can I update my meme after I've pushed it?**  
**A:** Yes! Simply make your changes, commit, and push again.  
Your live page and the competition website will update automatically.  

✅ You can even vote for your own meme! 🎉  

---

**Q: Can my team submit more than one meme?**  
**A:** The system displays one website per team.  
However, you can create a **multi-page meme site!**  
Just add more HTML files (e.g., `meme2.html`) and link to them from your main `index.html`.  

---

## 📜 Rules & Notes
- Please keep content **appropriate for all audiences**.  
- The use of **web technologies (HTML, CSS, JS)** is encouraged!  
- You may use **libraries and frameworks** if you wish.  

---

🎉 Good luck, have fun, and may the best meme win Odin's sacred runes!  

**Remember: In Git We Trust! 🚀**
