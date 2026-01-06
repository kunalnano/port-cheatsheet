# 🚀 Port.io Implementation Toolkit

<div align="center">

**Production-ready patterns and decision frameworks for Port.io implementations**

[![Live Site](https://img.shields.io/badge/Live-Cheat_Sheet-blue?style=for-the-badge)](https://kunalnano.github.io/port-cheatsheet/)
[![Mental Model](https://img.shields.io/badge/Live-Mental_Model-purple?style=for-the-badge)](https://kunalnano.github.io/port-cheatsheet/port-mental-model.html)
[![JQ Playground](https://img.shields.io/badge/Tool-JQ_Playground-cyan?style=for-the-badge)](https://jq.port.io/)

</div>

---

## 📚 What's Inside

| Resource | Description | Use When |
|----------|-------------|----------|
| [**Pattern Cheat Sheet**](https://kunalnano.github.io/port-cheatsheet/) | Copy-paste code snippets for blueprints, mappings, actions, scorecards, automations, JQ, and API calls | You know what you need — just need the syntax |
| [**Mental Model Guide**](https://kunalnano.github.io/port-cheatsheet/port-mental-model.html) | Decision trees and frameworks for *how to think* about Port implementations | You're unsure which approach to use |

---

## 🎯 Pattern Cheat Sheet

> **33 production-validated patterns** across 8 categories

### Categories

| Category | Patterns | Examples |
|----------|:--------:|----------|
| **Blueprints** | 5 | Basic schema, arrays/objects, mirror, calculation, aggregation |
| **Mapping** | 6 | GitHub, Kubernetes, ArgoCD, Terraform, search relations, webhooks |
| **Actions** | 5 | Self-service, entity selection, create entity, approval flows, webhooks |
| **Scorecards** | 3 | Production readiness, time-based rules, mirror properties |
| **Automations** | 4 | Entity created/updated, timer triggers, scorecard changes |
| **JQ** | 5 | Defaults, strings, arrays, dates, automation conditions |
| **API** | 5 | Auth, CRUD, search, action status, bulk operations |
| **Troubleshooting** | 4 | Missing entities, null values, broken relations, stuck actions |

### Features

- 🔍 **Search** — Find patterns by keyword (press `/` to focus)
- 🏷️ **Filter** — Click category tabs to narrow results
- 📋 **Copy** — One-click copy for any snippet
- 🔗 **Deep links** — Share direct links to specific patterns
- 🖨️ **Print** — Export to PDF for offline reference

---

## 🧭 Mental Model Guide

> **Think before you build** — Decision frameworks that prevent costly rework

### What You'll Learn

| Section | Key Question |
|---------|--------------|
| **Entity Test** | Should this be a Blueprint or just a Property? |
| **Granularity Matrix** | How deep should I model? (Cloud, K8s, Source Control, Security) |
| **Property Types** | Regular vs Mirror vs Calculation vs Aggregation? |
| **Relations** | When to use Relations vs Properties vs Search Relations? |
| **Actions vs Automations** | Human-triggered or event-driven? |
| **Scorecards** | Standards tracking vs simple properties? |
| **Anti-Patterns** | Common mistakes and how to avoid them |

### The Golden Rule

> **Only create a Blueprint if it meets 3 of 4 criteria:**
> 1. **Ownership** — Does a specific team own it?
> 2. **Lifecycle** — Independent of its parent?
> 3. **Workflow** — Will you run Day 2 Actions against it?
> 4. **Scorecard** — Need to track quality/compliance over time?

---

## 🛠️ Quick Start

### Option 1: Use Online
- **Cheat Sheet**: [kunalnano.github.io/port-cheatsheet](https://kunalnano.github.io/port-cheatsheet/)
- **Mental Model**: [kunalnano.github.io/port-cheatsheet/port-mental-model.html](https://kunalnano.github.io/port-cheatsheet/port-mental-model.html)

### Option 2: Use Offline
```bash
# Clone the repo
git clone https://github.com/kunalnano/port-cheatsheet.git

# Open in browser
open port-cheatsheet/index.html
```

Both pages are **single-file HTML with zero dependencies** — they work completely offline.

---

## 📝 File Reference

| File | Description |
|------|-------------|
| `index.html` | Pattern Cheat Sheet (default, no dependencies) |
| `index-prism.html` | Pattern Cheat Sheet with Prism.js syntax highlighting |
| `port-mental-model.html` | Mental Model decision guide |

---

## 🔗 Related Resources

| Resource | Link |
|----------|------|
| Port.io Documentation | [docs.port.io](https://docs.port.io) |
| Port.io API Reference | [api.getport.io/static/index.html](https://api.getport.io/static/index.html) |
| JQ Playground | [jq.port.io](https://jq.port.io/) |

### API Regions
- **US**: `api.getport.io`
- **EU**: `api.eu.getport.io`

---

## 🤝 Contributing

### Add a Pattern

Edit the `patterns` array in `index.html`:

```javascript
{
  id: 'unique-pattern-id',
  category: 'mapping',  // blueprints|mapping|actions|scorecards|automations|jq|api|troubleshooting
  title: 'Your Pattern Title',
  validated: 'tested',  // production|tested|adapt
  problem: 'What problem this solves',
  description: 'How it works',
  code: `your code here`,
  output: 'Expected result or notes',
  tags: ['tag1', 'tag2']
}
```

### Improve the Mental Model

Edit `port-mental-model.html` to add decision trees, anti-patterns, or granularity guidance.

---

## 📄 License

MIT — Use freely, attribution appreciated.

---

<div align="center">

**Built for Port.io practitioners** · Patterns validated in real implementations

[Open Cheat Sheet](https://kunalnano.github.io/port-cheatsheet/) · [Open Mental Model](https://kunalnano.github.io/port-cheatsheet/port-mental-model.html)

</div>
