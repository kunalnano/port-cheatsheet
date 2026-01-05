# Port.io Implementation Cheat Sheet

**Live Site:** [https://kunalnano.github.io/port-cheatsheet/](https://kunalnano.github.io/port-cheatsheet/)

Copy-paste patterns for Port.io blueprints, mappings, actions, scorecards, automations, JQ, and API calls.

---

## Versions

| File | Description | Dependencies |
|------|-------------|--------------|
| [`index.html`](index.html) | **Default** - Dependency-free, works offline | None |
| [`index-prism.html`](index-prism.html) | Enhanced syntax highlighting | Prism.js via CDN |

**Recommendation:** Use `index.html` for reliability in corporate/restricted networks. Use `index-prism.html` for better visual polish when CDN access is available.

---

## What's Included

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

---

## How to Use

1. **Search** - Type keywords like `kubernetes`, `webhook`, `jq time`
2. **Filter** - Click category buttons to narrow results
3. **Copy** - Click "Copy" button on any snippet
4. **Adapt** - Replace `<YOUR_ORG>`, `<YOUR_REPO>`, `<YOUR_DOMAIN>` placeholders
5. **Print** - Use the Print button for PDF/offline reference

---

## API Regions

- **US:** `api.getport.io`
- **EU:** `api.eu.getport.io`

---

## Contributing

To add a pattern, edit the `patterns` array in the HTML file:

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

---

## Links

- [Port.io Documentation](https://docs.port.io)
- [Port.io API Reference](https://api.getport.io/static/index.html)
