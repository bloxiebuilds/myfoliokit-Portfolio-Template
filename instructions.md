# 📖 FolioKit — Instructions

Welcome! This guide will walk you through everything you need to get your portfolio live in minutes. No coding experience required.

---

## 📋 Table of Contents

1. [Getting Started](#1-getting-started)
2. [Editing Your Info](#2-editing-your-info)
3. [Adding Projects](#3-adding-projects)
4. [Adding & Removing Skills](#4-adding--removing-skills)
5. [Changing Colors](#5-changing-colors)
6. [Updating Contact Info & Social Links](#6-updating-contact-info--social-links)
7. [Deploying to GitHub Pages](#7-deploying-to-github-pages)
8. [FAQ](#8-faq)

---

## 1. Getting Started

### Option A — Use the Template (Recommended)
1. Go to [github.com/bloxiebuilds/myfoliokit-Portfolio-Template](https://github.com/bloxiebuilds/myfoliokit-Portfolio-Template)
2. Click the green **"Use this template"** button
3. Name your new repo (e.g. `my-portfolio`)
4. Click **"Create repository"**

### Option B — Clone it manually
```bash
git clone https://github.com/bloxiebuilds/myfoliokit-Portfolio-Template.git
cd myfoliokit-Portfolio-Template
```

### Preview it locally
Just open `index.html` in your browser — no server needed!

---

## 2. Editing Your Info

Open `index.html` in any text editor (Notepad, VS Code, etc.)

### Your Name
Find this line in the `<nav>` section:
```html
<span class="nav-logo">YourName.</span>
```
Replace `YourName` with your actual name.

Find this line in the `<h1>` hero section:
```html
<h1>Hi, I'm <span>Your Name</span>.<br/>I build things.</h1>
```
Replace `Your Name` with your name and feel free to change `I build things.` to whatever fits you.

### Your Bio
Find the `<!-- Edit me! -->` comment in the About section and replace the placeholder text with your real bio.

### Your Location & Background
In the About section, find and update:
```html
<p><strong>🎓 Background</strong><br/>Add your education or background here.</p>
<p><strong>📍 Location</strong><br/>Your City, Country</p>
<p><strong>💼 Currently</strong><br/>What you're working on right now.</p>
```

---

## 3. Adding Projects

Find the Projects section and look for the `<!-- PROJECT CARD -->` comment. Copy and paste this block for each project:

```html
<a href="YOUR_PROJECT_LINK" class="project-card">
  <div class="project-icon">🔥</div>
  <h3>Project Name</h3>
  <p>A short description of what this project does and why it matters.</p>
  <span class="project-tag">View Project →</span>
</a>
```

**Tips:**
- Replace `YOUR_PROJECT_LINK` with a GitHub link, live site, or `#` if not ready
- Change the emoji in `project-icon` to something that fits the project
- Keep descriptions short — 1 to 2 sentences is perfect

---

## 4. Adding & Removing Skills

Find the Skills section and look for the `<div class="skills-grid">` block.

**To add a skill:**
```html
<span class="skill-tag">Your New Skill</span>
```

**To remove a skill:** just delete the full `<span class="skill-tag">...</span>` line.

---

## 5. Changing Colors

Near the top of `index.html`, find:
```css
--accent: #38BDF8;
```

Replace `#38BDF8` with any hex color you like. Here are some ideas:

| Color | Hex Code |
|-------|----------|
| Sky blue (default) | `#38BDF8` |
| Mint green | `#6EE7B7` |
| Soft purple | `#A78BFA` |
| Warm orange | `#FB923C` |
| Hot pink | `#F472B6` |
| Golden yellow | `#FBBF24` |

> 💡 Tip: Use [coolors.co](https://coolors.co) to find a color you love, then grab its hex code.

---

## 6. Updating Contact Info & Social Links

Find the Contact section and update your phone and email:

```html
<span class="social-link">📞 Phone: YOUR-NUMBER</span>
<span class="social-link">📧 Email: your@email.com</span>
```

Just replace `YOUR-NUMBER` and `your@email.com` with your real details.

### Social Links
Below the phone and email, update your social links:

```html
<a href="https://twitter.com/yourhandle" class="social-link">Twitter / X</a>
<a href="https://linkedin.com/in/yourprofile" class="social-link">LinkedIn</a>
```

**To add a new social link**, copy one of the lines above and change the URL and label:
```html
<a href="https://yoursite.com" class="social-link">Your Site</a>
```
**To remove a social link**, delete the full `<a ...>...</a>` line.

---

## 7. Deploying to GitHub Pages

This is how you get your portfolio live on the internet — **for free!**

1. Push your repo to GitHub (make sure it's public)
2. Go to your repo on GitHub
3. Click **Settings** (top menu)
4. Scroll down to **Pages** (left sidebar)
5. Under **Source**, select `main` branch and `/ (root)` folder
6. Click **Save**
7. Wait ~60 seconds, then visit:

```
https://YOUR-GITHUB-USERNAME.github.io/myfoliokit-Portfolio-Template
```

🎉 Your portfolio is live!

---

## 8. FAQ

**Q: Do I need to know how to code?**
No! All changes are simple text swaps. If you can edit a Word document, you can edit this template.

**Q: Can I use this for free?**
Yes — FolioKit is MIT licensed. Use it for personal or commercial projects, no credit required (though appreciated!).

**Q: How do I add a profile photo?**
In the About section, add this inside the second column:
```html
<img src="your-photo.jpg" style="width:100%;border-radius:12px;" alt="Your Name"/>
```
Put your photo file in the same folder as `index.html`.

**Q: Something looks broken — help!**
Make sure every tag you edited is still properly closed. For example `<h3>Title</h3>` not `<h3>Title`. When in doubt, undo your last change and try again.

**Q: Can I add more sections?**
Absolutely! Copy an existing `<section>` block, change the label number and content, and you're good to go.

---

<p align="center">Made with ❤️ by <a href="https://github.com/bloxiebuilds">bloxiebuilds</a></p>
