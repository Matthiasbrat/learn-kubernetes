# Kubernetes Documentation

A comprehensive documentation browser for learning Kubernetes from 0 to 100.

## 🚀 Live Demo

[Browse the Documentation](https://matthiasbrat.github.io/kubernetes-docs-extract/)

## ✨ Features

- **Two learning modes:**
  - 📖 **Learn** — Structured guide with 7 chapters and 46 sections
  - ❓ **Questions** — 49 Q&A organized across 8 categories
- **Full-text search** — Find answers instantly across both tabs
- **Personal investigations** — Includes deep dives into K8s internals
- **Code examples** — With YAML syntax highlighting
- **Dark/Light themes**
- **Font selection** — 7 fonts to choose from
- **Works offline** — Single HTML file

## 📖 Learn Guide Chapters

1. **Introduction** — What is Kubernetes, cluster architecture, components
2. **Core Concepts** — Objects, manifests, labels, namespaces, annotations
3. **Containers & Workloads** — Pods, lifecycle, init/sidecar containers, deployments
4. **Architecture Deep Dive** — API, nodes, controllers, CRI, garbage collection
5. **Scheduling & Resources** — Pod scheduling, disruptions, QoS, Downward API
6. **Production Setup** — kubeadm, HA, multi-zone, PKI, container runtimes
7. **Advanced Topics** — Ephemeral containers, user namespaces, finalizers, cgroups

## ❓ Questions Categories

1. **Getting Started** — What is Kubernetes, components, objects
2. **Core Concepts** — Labels, namespaces, annotations, finalizers
3. **Architecture** — API, nodes, controllers, CRI, garbage collection
4. **Workloads** — Pods, lifecycle, init/sidecar containers, deployments
5. **Scheduling** — Pod scheduling, disruptions, QoS classes
6. **Production Setup** — HA, multi-zone, large clusters, security
7. **Advanced Topics** — Downward API, user namespaces, leases
8. **Resources** — Useful links and references

## 🔍 Investigation Notes

This documentation includes personal investigation notes marked with badges:

| Badge | Meaning |
|-------|---------|
| 🔍 Investigation | Hands-on exploration and discoveries |
| 🏊 Deep Dive | Source code analysis |
| 📚 Reference | Cheat sheets and links |

Examples:
- How does kubelet know which node it belongs to?
- Why is kubelet a service but kube-proxy a container?
- How do informers and listers reduce API server load?

## 🛠️ Files

```
├── index.html                  # Redirect to browser
├── docs-browser-v2.html        # The documentation browser
├── learn-guide.json            # Learn tab content (7 chapters)
├── summary-restructured.json   # Questions tab content (49 questions)
└── README.md                   # This file
```

## 📝 Contributing

To add or update documentation:

1. Edit `learn-guide.json` for the Learn tab
2. Edit `summary-restructured.json` for the Questions tab
3. Follow the JSON schemas below
4. Submit a PR

### Learn Guide Schema

```json
{
  "chapter": "Chapter Name",
  "order": 1,
  "description": "What this chapter covers",
  "sections": [
    {
      "title": "Section Title",
      "content": "Content with **markdown** support.",
      "source": "https://source-link.com"
    }
  ]
}
```

### Questions Schema

```json
{
  "category": "Category Name",
  "order": 1,
  "topics": [
    {
      "question": "Your question?",
      "answer": "Short answer.",
      "details": "Longer explanation with **markdown**.",
      "source": "https://source-link.com",
      "type": "investigation"
    }
  ]
}
```

## 🔗 Related

- [Official Kubernetes Docs](https://kubernetes.io/docs/)
- [Kubernetes GitHub](https://github.com/kubernetes/kubernetes)

## 📜 License

MIT
