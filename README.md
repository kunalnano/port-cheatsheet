# Port.io Implementation Cheat Sheet

A quick-reference guide for Port.io implementation patterns, code snippets, and configurations.

## 🚀 Live Site

Once deployed, your cheat sheet will be available at:
```
https://<your-username>.github.io/port-cheatsheet/
```

## 📁 Repository Structure

```
port-cheatsheet/
├── index.html      # The cheat sheet (single-file app)
├── README.md       # This file
└── .nojekyll       # Tells GitHub Pages to serve files directly
```

## 🛠️ Setup Instructions

### 1. Create GitHub Repository

```bash
# Option A: GitHub CLI
gh repo create port-cheatsheet --public --source=. --push

# Option B: Manual
# 1. Go to github.com/new
# 2. Name it "port-cheatsheet"
# 3. Keep it public (required for free GitHub Pages)
# 4. Don't initialize with README (we already have files)
```

### 2. Push to GitHub

```bash
git add .
git commit -m "Initial commit: Port.io cheat sheet"
git remote add origin git@github.com:<YOUR_USERNAME>/port-cheatsheet.git
git push -u origin main
```

### 3. Enable GitHub Pages

1. Go to your repo on GitHub
2. Click **Settings** → **Pages** (left sidebar)
3. Under "Source", select:
   - **Branch:** `main`
   - **Folder:** `/ (root)`
4. Click **Save**
5. Wait 1-2 minutes for deployment

Your site will be live at `https://<your-username>.github.io/port-cheatsheet/`

## 🔄 Updating Content

Edit `index.html` and push:

```bash
git add index.html
git commit -m "Add new pattern: <description>"
git push
```

GitHub Pages auto-deploys on push (usually within 1-2 minutes).

## 🔒 Making it Private (GitHub Enterprise)

If you want to restrict access to your org only:

1. Use a **private repo** (requires GitHub Enterprise or Team)
2. In Settings → Pages, set visibility to "Private"
3. Only authenticated org members can view

## 📝 Adding New Patterns

Patterns are defined in the `patterns` array in `index.html`. Add new entries like:

```javascript
{
    category: 'blueprints',  // blueprints | mapping | actions | scorecards | automations | jq | api
    title: 'Pattern Name',
    description: 'What this pattern does',
    code: `your code here`,
    tags: ['tag1', 'tag2']
}
```

## 🤝 Contributing

1. Fork the repo
2. Add your pattern
3. Submit a PR

---

Built for the Port.io TSM team 🚢
