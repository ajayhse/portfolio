# Ajay Mishra — AI Portfolio Website

Live AI-powered portfolio chatbot. Visitors can chat with an AI that answers questions about your experience, skills, projects, and personal life.

---

## 🚀 Deploy to GitHub Pages (Free Hosting) — Step by Step

### Step 1: Add your profile photo

Put your photo file in this folder and name it exactly:
```
profile.jpg
```
(The one from your Eiffel Tower selfie works great!)

---

### Step 2: Create a GitHub repository

1. Go to https://github.com/new
2. Name it: `portfolio` (or `ajayhse.github.io` for a custom URL — see Step 6)
3. Set it to **Public**
4. Click **Create repository** (do NOT add README — leave it empty)

---

### Step 3: Push your files

Open your terminal (Mac/Linux) or Git Bash (Windows), then run:

```bash
# Navigate to this folder
cd path/to/ajay-portfolio

# Initialize git
git init

# Add all files
git add .

# First commit
git commit -m "Launch AI portfolio site"

# Connect to your GitHub repo (replace YOUR_USERNAME with ajayhse)
git remote add origin https://github.com/ajayhse/portfolio.git

# Push
git branch -M main
git push -u origin main
```

---

### Step 4: Enable GitHub Pages

1. Go to your repo on GitHub: `https://github.com/ajayhse/portfolio`
2. Click **Settings** (top right tab)
3. In the left sidebar, click **Pages**
4. Under **Source**, select **Deploy from a branch**
5. Branch: `main` | Folder: `/ (root)`
6. Click **Save**

Wait ~60 seconds, then your site is live at:
```
https://ajayhse.github.io/portfolio
```

---

### Step 5 (Optional): Use a custom domain

To use `ajaymishra.com` or similar:
1. Buy a domain (Namecheap, GoDaddy, etc.)
2. In GitHub Pages settings → **Custom domain**, enter your domain
3. In your domain's DNS settings, add these records:
   ```
   A     @   185.199.108.153
   A     @   185.199.109.153
   A     @   185.199.110.153
   A     @   185.199.111.153
   CNAME www ajayhse.github.io
   ```
4. Check **Enforce HTTPS**

---

### Step 6 (Optional): Use `ajayhse.github.io` as your URL (no /portfolio)

1. Rename the repo to exactly: `ajayhse.github.io`
2. Your site will be live at: `https://ajayhse.github.io`

---

## 📁 File Structure

```
ajay-portfolio/
├── index.html       ← Main portfolio + chat (all in one file)
├── profile.jpg      ← YOUR PHOTO (you must add this!)
└── README.md        ← This guide
```

---

## ✏️ How to update your site

```bash
# Make edits to index.html
git add .
git commit -m "Update portfolio"
git push
```
GitHub Pages auto-deploys in ~30 seconds.

---

## 📊 View Question Analytics

Scroll to the bottom of your live site — there's a **"Questions Asked Today"** section that logs every question visitors ask in real-time (session-based).

To add persistent question tracking across sessions, consider:
- Adding a free [Supabase](https://supabase.com) database
- Or using [Google Sheets API](https://developers.google.com/sheets/api) as a backend

---

## 🔧 Customize

Open `index.html` and search for:
- `ajaymishrahiet@gmail.com` → your email
- `profile.jpg` → your photo filename
- The `SYS` constant (JavaScript) → edit Ajay's bio/knowledge base

---

Built with ❤️ using HTML, CSS, vanilla JS, and Claude AI.
