# Port.io Implementation Cheat Sheet

**Live Site:** https://kunalnano.github.io/port-cheatsheet/

Copy-paste patterns for Port.io blueprints, mappings, actions, scorecards, automations, JQ, and API calls.

---

## Pages

| Page | Description | Use When |
|------|-------------|----------|
| [`index.html`](https://kunalnano.github.io/port-cheatsheet/) | **Pattern Cheat Sheet** — Copy-paste snippets | You know what you need, just need the syntax |
| [`mental-model.html`](https://kunalnano.github.io/port-cheatsheet/mental-model.html) | **Mental Model Guide** — Decision frameworks | You're deciding *what* to build, not just *how* |

---

## Versions (Cheat Sheet)

| File | Description | Dependencies |
|------|-------------|--------------|
| `index.html` | **Default** - Dependency-free, works offline | None |
| `index-prism.html` | Enhanced syntax highlighting | Prism.js via CDN |

**Recommendation:** Use `index.html` for reliability in corporate/restricted networks.

---

## What's Included

### Pattern Cheat Sheet (index.html)

| Category | Patterns | Examples |
|----------|----------|----------|
| **Blueprints** | 5 | Basic, arrays/objects, mirror, calculation, aggregation |
| **Mapping** | 6 | GitHub, K8s, ArgoCD, Terraform, search relations, webhooks |
| **Actions** | 5 | Self-service, entity selection, create, approval, workflows |
| **Scorecards** | 3 | Production readiness, time-based rules, mirror properties |
| **Automations** | 4 | Entity created/updated, cron/timer, scorecard triggers |
| **JQ** | 5 | Defaults, strings, arrays, dates, automation conditions |
| **API** | 5 | Auth, CRUD, search, run updates, bulk operations |

**Total: 33 patterns**

### Mental Model Guide (mental-model.html)

| Section | Content |
|---------|---------|
| **Entity Test** | The 3-of-4 Golden Rule for when to create a Blueprint |
| **Granularity Matrix** | Cloud, K8s, Source Control, Security — what to model vs. aggregate |
| **Decision Trees** | Property types, Relations, Actions vs Automations, Scorecards, Integrations |
| **Anti-Patterns** | Common mistakes that cause rework |
| **Implementation Phases** | 7-phase build sequence |

---

## How to Use

### Cheat Sheet
1. **Search** - Type keywords like `kubernetes`, `webhook`, `jq time`
2. **Filter** - Click category buttons to narrow results
3. **Copy** - Click "Copy" button on any snippet
4. **Adapt** - Replace `<YOUR_ORG>`, `<YOUR_REPO>`, `<YOUR_DOMAIN>` placeholders

### Mental Model
1. **Navigate** - Use sidebar to jump to sections
2. **Expand** - Click decision tree cards to see flowcharts
3. **Decide** - Follow the logic to pick the right approach
4. **Print** - Use Print button for offline/PDF reference

---

## API Regions

* **US:** `api.getport.io`
* **EU:** `api.eu.getport.io`

---

## Contributing

### Add a Pattern (Cheat Sheet)
Edit the `patterns` array in `index.html`:

```javascript
{
    category: 'mapping',           // blueprints|mapping|actions|scorecards|automations|jq|api
    title: 'Your Pattern Title',
    problem: 'What problem this solves',
    description: 'How it works',
    code: `your code here`,
    output: `expected result or notes`,
    tags: ['tag1', 'tag2']
}
```

### Improve Mental Model
Edit `mental-model.html` directly. Key sections:
- Decision trees use `.tree` class with semantic spans (`.q`, `.yes`, `.no`, `.result`)
- Tables use standard HTML with badge classes (`.badge-green`, `.badge-yellow`, `.badge-red`)
- Collapsible cards use `.card` with click handler on `.card-header`

---

## Links

* [Port.io Documentation](https://docs.port.io)
* [Port.io API Reference](https://api.getport.io/static/index.html)
