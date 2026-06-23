---
> 🚀 **Trial v0.30.0 is live!** The latest release is available for trial today — [get started in 5 minutes →](#try-v030-in-5-minutes)

# Hermes — Community

> **Application operating layer for Kubernetes — auto-discover every dashboard and tool, one permanent front door.**

![Version](https://img.shields.io/badge/version-v0.30.0-blue) ![Discussions](https://img.shields.io/github/discussions/hypersdk/hermes-community) ![Issues](https://img.shields.io/github/issues/hypersdk/hermes-community) ![License](https://img.shields.io/badge/license-Proprietary-red)

Public issue tracker and community feedback space for **Hermes** by [Zyvor AI Labs](https://zyvor.dev).
The source code is maintained in a private repository. This repo is for bug reports, feature requests, UX feedback, and community discussion.

---

## What's new in v0.30

- Spotlight NL search GA — find any app, pod, or service by describing it in plain English
- Zeus AI health summary — explains cluster-wide health issues in plain language, no kubectl required
- App catalog export — export your discovered app catalog to JSON or a static site
- Helm v0.30 — single-chart install with cert-manager integration and ingress auto-config
- Annotation-free discovery — Hermes now infers app purpose from service names and port conventions

---

## Why Hermes

| Problem | Hermes answer |
|---------|--------------|
| "Where is Grafana?" every Monday morning | Living app catalog — every tool auto-discovered and permanently linked |
| Bookmark sprawl and tribal cluster knowledge | Permanent URLs — the cluster self-documents, no maintenance needed |
| Port-forward culture slows every developer | Gateway front door to every workload — one URL, always on |
| Raw probe errors need namespace archaeology | Zeus AI explains fleet health in plain language — no kubectl expertise needed |
| New team members take weeks to find their tools | macOS Launchpad UX — every app is one click from the home screen |

---

## Architecture

```
┌──────────────────────────────────────────────────────────────┐
│  Experience   Launchpad · App catalog · Health · Gateway     │
├──────────────────────────────────────────────────────────────┤
│  Discovery    Continuous cluster scan · annotation-aware     │
├──────────────────────────────────────────────────────────────┤
│  Zeus AI      Fleet insight · Spotlight NL · diagnose flows  │
└──────────────────────────────────────────────────────────────┘
```

---

## Try v0.30 in 5 minutes

```bash
helm repo add hypersdk https://charts.hypersdk.dev
helm install hermes hypersdk/hermes --version 0.30.0 \
  -n hermes-system --create-namespace \
  --set global.domain=your-cluster.local
```

Hermes begins scanning immediately. Open the Launchpad UI at your configured domain — no further configuration needed.

**Requirements:** Kubernetes 1.28+, DNS or ingress configured for your cluster domain

---

## Report a bug

[Open a Bug Report →](../../issues/new?template=bug_report.yml)

Include: what you did, what happened, what you expected, your environment, screenshots or logs (redact secrets).

## Request a feature

[Open a Feature Request →](../../issues/new?template=feature_request.yml)

## UX feedback

[Open a UX Report →](../../issues/new?template=ux_feedback.yml)

## Ask a question

Use [GitHub Discussions](../../discussions) for open-ended questions, ideas, and roadmap conversations.

---

## Security

**Do not report security vulnerabilities publicly.**
Email **security@zyvor.dev** — see [SECURITY.md](SECURITY.md).

---

## Do not post

- Source code, internal configs, or architecture details
- API tokens, license keys, or credentials
- Private logs with sensitive data
- Security vulnerabilities — email security@zyvor.dev instead

---

## Join the community

⭐ [Star this repo](https://github.com/hypersdk/hermes-community) · 💬 [Open a Discussion](https://github.com/hypersdk/hermes-community/discussions) · 🐛 [Report a Bug](../../issues/new?template=bug_report.yml) · 📧 [hello@zyvor.dev](mailto:hello@zyvor.dev)

Maintained by [Zyvor AI Labs](https://zyvor.dev)
