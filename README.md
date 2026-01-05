# Port.io Implementation Cheat Sheet

Quick-reference patterns for Port.io implementations. Copy-paste ready.

## 🔗 [**Open the Cheat Sheet →**](https://kunalnano.github.io/port-cheatsheet/)

---

## What's Inside

| Category | Patterns | Use For |
|----------|----------|---------|
| **Blueprints** | Properties, mirrors, calculations, aggregations | Designing data models |
| **Mapping** | JQ transforms, search relations, ArgoCD, K8s | Integration configuration |
| **Actions** | Self-service, GitHub workflows, webhooks, RBAC | Building developer workflows |
| **Scorecards** | Production readiness, security, time-based rules | Compliance & standards |
| **Automations** | Entity triggers, timers, Slack/Jira notifications | Event-driven workflows |
| **JQ Patterns** | Common expressions, conditionals, time calcs | Writing JQ anywhere in Port |
| **API** | REST examples, Python SDK | Programmatic access |

## How to Use

1. **Search** - Type keywords to filter across all patterns
2. **Filter** - Click category buttons to narrow down
3. **Copy** - Hit the copy button on any snippet
4. **Adapt** - Replace `<YOUR_ORG>`, `<YOUR_REPO>`, etc. with actual values

## API Region Note

Snippets use `api.getport.io` (US). For EU customers, swap to `api.eu.getport.io`.

## Contributing

Add patterns directly to the `patterns` array in `index.html`:

```javascript
{
    category: 'actions',  // blueprints | mapping | actions | scorecards | automations | jq | api
    title: 'Your Pattern Name',
    description: 'What it does',
    code: `your code here`,
    tags: ['relevant', 'tags']
}
```

PR it or ping moi.

---

Built for Port.io customer implementations 🚢
