# 🚀 RepoRefine

🔗 **Live Demo:** https://repo-refine.vercel.app/

**RepoRefine** is a GitHub profile and repository audit tool that analyzes profiles, repository links, activity patterns, tech stacks, README quality, and project health to detect weaknesses and generate actionable improvements — making your GitHub presence recruiter-ready.

RepoRefine combines deterministic GitHub GraphQL checks with optional Groq-powered review summaries so scoring stays transparent while recommendations can still feel personalized.

---

## ✨ Features

### 🔍 Profile Audit
- Profile completeness analysis
- Bio strength check
- Pinned repo validation
- Branding score
- Recruiter impression score

### 📂 Repository Health Analysis
- Analyze a single GitHub repository from its URL
- Tech stack detection from languages, manifests, config files, topics, Docker, and CI signals
- README quality scoring with detected and missing sections
- License detection
- Maintenance activity check
- Open issue count detection
- CI/CD presence detection
- Test folder detection
- Documentation scoring
- Feature and update recommendations for the given repository

### 📊 Commit & Activity Analysis
- Commit consistency detection
- Inactivity gap detection
- Commit message hygiene scoring
- Commit chronotype analysis

### 📈 Scoring System
- Profile Health Score (0–100)
- Repository Health Score
- Documentation Score
- Consistency Score
- Recruiter Readiness Index

### 📊 Visual Dashboard
- Radar skill graph
- Health score meter
- Repository audit cards
- Red/Yellow/Green indicators
- Commit heatmap visualization

---

## 🛠 Tech Stack

- **Frontend:** Next.js (App Router)
- **Styling:** Tailwind CSS
- **Charts:** Recharts
- **API:** GitHub GraphQL API and optional Groq API
- **Auth:** GitHub Personal Access Token

---

## 🚀 Getting Started

### 1️⃣ Clone the repository

```bash
git clone https://github.com/Sushma-1706/RepoRefine.git
cd RepoRefine
```
### 2️⃣ Install dependencies
```bash
npm install
```
### 3️⃣ Add Environment Variables
Create a .env.local file:
``` bash
GITHUB_TOKEN=your_github_pat_token
GROQ_API_KEY=your_groq_api_key_optional
```
### 4️⃣ Run locally
```bash
npm run dev
```
App runs at:
```bash
http://localhost:3000
```
---

### 🧠 How It Works
RepoRefine uses GitHub GraphQL queries to fetch:
- Profile metadata
- Repository data
- Commit history
- Issues & pull requests
- Then it applies deterministic audit logic to:
- Detect weaknesses
- Calculate scores
- Generate structured improvement suggestions
- Identify the tech stack and README improvements for a pasted GitHub repository URL

If `GROQ_API_KEY` is configured, RepoRefine can also generate persona-based review commentary for profile audits.

### 📦 Future Enhancements
- PDF export mode
- Before vs After improvement comparison
- Recruiter bulk candidate mode
- Open-source scoring benchmark
 ---
### 📜 License
MIT License
