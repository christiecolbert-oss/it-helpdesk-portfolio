# 🐙 GitHub + Netlify Step-by-Step Deploy Guide

## STEP 1 — Create Your GitHub Repo

1. Go to **github.com** and sign in
2. Click the **+** icon → **New repository**
3. Fill in:
   - **Repository name:** `it-helpdesk-portfolio`
   - **Description:** `IT Help Desk & Sysadmin Portfolio — AD, Jira, Zendesk simulations`
   - Set to **Public** (hiring managers need to see it)
   - ✅ Check **Add a README file** → NO (we have our own)
4. Click **Create repository**

---

## STEP 2 — Push Your Code

Open your terminal in the project folder:

```bash
git init
git add .
git commit -m "feat: initial commit — IT portfolio with AD, helpdesk, ticket, and asset modules"
git remote add origin https://github.com/YOUR_USERNAME/it-helpdesk-portfolio.git
git branch -M main
git push -u origin main
```

✅ Verify your files appear on GitHub at `github.com/YOUR_USERNAME/it-helpdesk-portfolio`

---

## STEP 3 — Connect to Netlify

1. Go to **app.netlify.com** → Sign up/in with GitHub
2. Click **Add new site** → **Import an existing project**
3. Click **GitHub** and authorize Netlify
4. Search for and select **it-helpdesk-portfolio**
5. Configure build settings:
   ```
   Branch to deploy:  main
   Build command:     npm run build
   Publish directory: dist
   ```
6. Click **Deploy site**

Netlify will give you a URL like `random-name-123.netlify.app`

---

## STEP 4 — Custom Site Name (Free)

1. In Netlify → **Site settings** → **General**
2. Click **Change site name**
3. Set it to: `yourname-it-portfolio`
4. Your URL becomes: `yourname-it-portfolio.netlify.app`

Put this URL on your resume and LinkedIn!

---

## STEP 5 — Set Up Auto-Deploy (CI/CD)

This is already done! Every time you push to `main`:
- Netlify detects the push
- Runs `npm run build`
- Deploys the new version automatically

To test it:
```bash
# Make a small change, then:
git add .
git commit -m "fix: update dashboard stats"
git push
# Watch Netlify auto-deploy at app.netlify.com
```

---

## STEP 6 — GitHub Best Practices for Portfolio

### Write Good Commit Messages
```bash
# Good examples:
git commit -m "feat: add ticket priority filtering to kanban board"
git commit -m "fix: resolve AD user lock/unlock toggle bug"
git commit -m "docs: update README with Netlify deploy instructions"
git commit -m "style: improve help desk mobile responsiveness"

# Bad examples:
git commit -m "update"
git commit -m "stuff"
git commit -m "fix bug"
```

### Use Branches for Features
```bash
git checkout -b feature/add-asset-qr-codes
# ... do your work ...
git add .
git commit -m "feat: add QR code generation for asset tags"
git push origin feature/add-asset-qr-codes
# Then open a Pull Request on GitHub
```

### Pin This Repo on Your GitHub Profile
1. Go to your GitHub profile
2. Click **Customize your pins**
3. Select `it-helpdesk-portfolio`
4. Add a good description and topics:
   - Topics: `active-directory`, `helpdesk`, `jira`, `zendesk`, `react`, `itsm`, `it-portfolio`

---

## STEP 7 — Add a GitHub Profile README

Create a special repo named exactly your username (e.g., `johndoe/johndoe`) with a `README.md`:

```markdown
# Hi, I'm [Your Name] 👋

🖥️ IT Systems Administrator | Help Desk | Sysadmin

## 🛠️ Skills
- Active Directory, Group Policy, DNS/DHCP
- Help Desk & Ticketing (Jira, Zendesk)
- IT Asset Management
- Windows Server, PowerShell
- React, JavaScript, CI/CD

## 📌 Featured Projects
- [IT Help Desk Portfolio](https://github.com/YOUR_USERNAME/it-helpdesk-portfolio) — Full IT ops simulation
```

---

## Resume Tips

Add this to your resume under **Projects**:

```
IT Help Desk & Sysadmin Portfolio                          [Live Demo Link] | [GitHub Link]
- Built a full-stack IT operations dashboard simulating Active Directory, Jira, and Zendesk workflows
- Implemented user lifecycle management, ticket SLA tracking, and IT asset inventory modules
- Deployed via Netlify with automated CI/CD pipeline connected to GitHub
- Tech: React, JavaScript, Git, Netlify
```
