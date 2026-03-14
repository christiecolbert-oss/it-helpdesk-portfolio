🖥️ IT Help Desk & Systems Administration Portfolio
A full-stack simulation of enterprise IT tools built to demonstrate real-world sysadmin, help desk, and IT operations skills.
Built by [Christie Colbert] | [Christie,Colbert@gmail.com] | [(https://www.linkedin.com/in/christie-colbert/)]
�
Load image
🚀 Live Demo
🔗 [(https://app.netlify.com/teams/christie-colbert/projects)]
🛠️ Tech Stack
Layer
Technology
Frontend
React 18, JavaScript (ES2022)
Styling
CSS-in-JS, Google Fonts
Deployment
Netlify (CI/CD from GitHub)
Version Control
Git / GitHub
Simulated Integrations
Active Directory, Zendesk, Jira
📋 Modules & Skills Demonstrated
1. 🎫 Ticket Management (Jira-style)
Create, assign, prioritize, and resolve IT support tickets
Kanban board + list view
SLA countdown timers
Priority levels: Critical / High / Medium / Low
Skills: ITSM workflows, incident management, Jira-equivalent concepts
2. 🎧 Help Desk Portal (Zendesk-style)
Customer-facing ticket submission form
Agent queue with status management
Canned responses & internal notes
CSAT tracking
Skills: End-user support, ticketing SLAs, Zendesk-equivalent workflows
3. 🗂️ Active Directory Console
User account creation, deletion, lock/unlock
Organizational Unit (OU) management
Security group assignment
Security event log viewer (4624, 4625, 4740 events)
Skills: Windows Server AD, LDAP, user lifecycle management
4. 💻 Asset Inventory
Hardware asset tracking (laptops, monitors, peripherals)
Check-in / check-out system
Asset assignment to users
Warranty & lifecycle tracking
Skills: ITAM (IT Asset Management), CMDB concepts
5. 📊 IT Dashboard
Live KPIs: open tickets, avg resolution time, asset utilization
Ticket trend charts
Recent activity feed
Skills: IT metrics, reporting, KPI tracking
🚀 Getting Started
Prerequisites
Node.js v18+
npm or yarn
Git
Local Setup
# 1. Clone the repository
git clone https://github.com/YOUR_USERNAME/it-portfolio.git

# 2. Navigate into the project
cd it-portfolio

# 3. Install dependencies
npm install

# 4. Start development server
npm run dev

# 5. Open in browser
# http://localhost:5173
📦 Deploying to Netlify
Option A: Netlify Drop (Fastest — no CLI needed)
Run npm run build locally
Go to app.netlify.com/drop
Drag and drop your dist/ folder
✅ Live in 30 seconds
Option B: GitHub + Netlify CI/CD (Recommended for portfolio)
Push your code to GitHub
Go to app.netlify.com → Add new site → Import from Git
Connect your GitHub account and select this repo
Set build settings:
Build command: npm run build
Publish directory: dist
Click Deploy site
Every push to main will auto-deploy ✅
Option C: Netlify CLI
npm install -g netlify-cli
netlify login
netlify init
netlify deploy --prod
🐙 Pushing to GitHub
# Initialize git (if not already done)
git init

# Add all files
git add .

# First commit
git commit -m "feat: initial IT portfolio with AD, helpdesk, tickets, and asset modules"

# Create repo on GitHub (github.com → New Repository)
# Then connect it:
git remote add origin https://github.com/YOUR_USERNAME/it-portfolio.git
git branch -M main
git push -u origin main
Recommended Branch Strategy
main          → production (auto-deploys to Netlify)
dev           → development work
feature/xxx   → individual features
📁 Project Structure
it-portfolio/
├── public/
│   └── favicon.ico
├── src/
│   ├── components/
│   │   ├── Dashboard.jsx       # KPI overview
│   │   ├── TicketBoard.jsx     # Jira-style tickets
│   │   ├── HelpDesk.jsx        # Zendesk-style portal
│   │   ├── ADConsole.jsx       # Active Directory UI
│   │   └── AssetInventory.jsx  # Hardware asset tracker
│   ├── data/
│   │   └── mockData.js         # Seed data for all modules
│   ├── App.jsx
│   └── main.jsx
├── docs/
│   ├── screenshots/
│   ├── DEPLOY.md
│   └── SKILLS.md
├── .gitignore
├── package.json
├── vite.config.js
└── README.md
🗺️ Roadmap
[ ] Backend API with Node.js / Express
[ ] Real authentication (JWT)
[ ] PostgreSQL database integration
[ ] PowerShell script integration for AD automation
[ ] Email notifications via SendGrid
[ ] Slack webhook alerts for critical tickets
[ ] Dark/Light mode toggle
[ ] Mobile responsive layout
📸 Screenshots
Module
Preview
Dashboard
(Add screenshot)
Ticket Board
(Add screenshot)
Help Desk
(Add screenshot)
AD Console
(Add screenshot)
Asset Inventory
(Add screenshot)
🧠 Skills This Project Demonstrates
Active Directory — User management, OUs, groups, security event log
ITSM / Help Desk — Ticket lifecycle, prioritization, SLA management
Jira — Kanban boards, issue tracking, sprint-style workflow
Zendesk — Agent queues, canned responses, CSAT, ticket escalation
IT Asset Management — Hardware lifecycle, check-in/out, assignment
CI/CD — GitHub → Netlify automatic deployments
React — Component-based UI development
Documentation — README, setup guides, deployment docs
📄 License
MIT License — feel free to fork and adapt for your own portfolio.
Built as a portfolio project to demonstrate IT systems administration and help desk skills.
