# How to Upload This Brand Kit to GitHub

This guide walks you through setting up your brand kit repository on GitHub in 5 minutes.

---

## STEP 1: Create a GitHub Account (if you don't have one)

1. Go to **github.com**
2. Click "Sign up"
3. Complete the registration with your email
4. Verify your email

---

## STEP 2: Create a New Repository

1. Log into GitHub
2. Click the **+** icon in top right → **New repository**
3. Fill in:
   - **Repository name:** `THE-INK-MOON-BRAND-KIT`
   - **Description:** "Brand guidelines, pricing, proposals, and assets for The Ink Moon design projects"
   - **Visibility:** Choose **Private** (only you can see) or **Public** (anyone can view)
   - **Add .gitignore:** Choose "None" (we don't need it)
   - **Add License:** Choose "None" (or MIT if you prefer)

4. Click **Create repository**

---

## STEP 3: Download & Install Git

1. Go to **git-scm.com**
2. Download the version for your operating system (Mac/Windows/Linux)
3. Install it (click through all defaults)
4. Open Terminal/Command Prompt and verify:
   ```
   git --version
   ```

---

## STEP 4: Clone the Repository to Your Computer

1. On GitHub, your new repo page shows a green **Code** button
2. Click it and copy the HTTPS link (it looks like: `https://github.com/yourname/THE-INK-MOON-BRAND-KIT.git`)
3. Open Terminal/Command Prompt and run:
   ```
   git clone https://github.com/yourname/THE-INK-MOON-BRAND-KIT.git
   ```
   (Replace `yourname` with your actual GitHub username)

4. Navigate into the folder:
   ```
   cd THE-INK-MOON-BRAND-KIT
   ```

---

## STEP 5: Add All the Brand Kit Files

I've prepared all the files for you. Here's what you'll add:

**Files Already Created:**
- `README.md` — Master brand guide
- `BRAND_GUIDELINES/Brand_Guidelines.md` — Voice, visual style, principles
- `BRAND_GUIDELINES/Pricing_Pricing_Sheets.json` — All pricing data
- `BRAND_GUIDELINES/Terms_Conditions.md` — Legal terms
- `TEMPLATES/Hotel_Proposal_Template.md` — Hotel proposal structure
- `TEMPLATES/Corporate_Proposal_Template.md` — Corporate proposal structure

**You'll need to add:**
- Logo files (`.png` or `.svg`) → Move to `ASSETS/`
- Color palette reference image → `ASSETS/`
- Sample artwork images → `ASSETS/`
- Your PDF documents (compressed) → `CATALOGUES/`

---

## STEP 6: Add & Commit Files

In Terminal, from within the repository folder:

```bash
# Add all files
git add .

# Commit with a message
git commit -m "Initial brand kit: guidelines, pricing, and proposal templates"

# Push to GitHub
git push origin main
```

When it asks for authentication:
- **Username:** Your GitHub username
- **Password:** Your GitHub personal access token (see below)

---

## STEP 7: Create a GitHub Personal Access Token (Authentication)

GitHub no longer accepts plain passwords. You need a Personal Access Token:

1. Go to GitHub → **Settings** (top right menu)
2. Click **Developer settings** (bottom left)
3. Click **Personal access tokens** → **Tokens (classic)**
4. Click **Generate new token (classic)**
5. Fill in:
   - **Note:** `The Ink Moon Brand Kit`
   - **Expiration:** 90 days (or longer)
   - **Select scopes:** Check `repo` (full control of private repositories)
6. Click **Generate token**
7. **Copy the token immediately** (you won't see it again)
8. Paste this token when Git asks for your password

---

## STEP 8: Verify Upload

1. Refresh your GitHub repository page
2. You should see all your files listed
3. The README will display automatically

✅ **Done! Your brand kit is now on GitHub.**

---

## How Claude Design Uses This

When you connect Claude Design to this GitHub repo:

1. I can read all markdown files and extract:
   - Pricing structures
   - Brand guidelines
   - Proposal templates
   - Terms & conditions

2. I can reference this in future projects to:
   - Maintain consistent pricing
   - Apply brand voice & visual style
   - Use proposal templates as starting points
   - Ensure legal compliance

3. You can update the repo anytime and I'll have the latest info

---

## Keeping Your Brand Kit Updated

Whenever you update prices, add new templates, or modify guidelines:

```bash
# Make your changes in the files
# Then:

git add .
git commit -m "Update: [describe what changed]"
git push origin main
```

---

## Optional: Make It More Discoverable

Add a **Topics** tag to your repo so it's easy to find:

1. On your GitHub repo page, click **About** (top right)
2. Add topics like: `art`, `brand-kit`, `design`, `proposals`
3. Save

---

## Need Help?

- **Git isn't working?** Try: `git status` to see what's happening
- **Can't authenticate?** Make sure you used the Personal Access Token, not your password
- **Files aren't showing?** Make sure they're in the folder before pushing

---

## Summary

```
1. Create GitHub account → github.com/signup
2. Create new repository (name: THE-INK-MOON-BRAND-KIT)
3. Install Git → git-scm.com
4. Clone repo → git clone [your-repo-url]
5. Add files (I've prepared most of them)
6. Commit & Push → git add . + git commit + git push
7. Verify files appear on GitHub
```

**Total time: 5-10 minutes**

---

**Next:** Tell Claude Design the GitHub repo URL, and I can use it for all future projects! 🚀
