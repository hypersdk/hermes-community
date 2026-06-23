# Hermes — Community

> **Application operating layer for Kubernetes — auto-discover every dashboard and tool, one front door**

Public issue tracker and community feedback space for **Hermes** by [Zyvor AI Labs](https://zyvor.dev).

The source code is maintained in a private repository. This repo is for:
- Bug reports
- Feature requests
- UX feedback
- Documentation gaps
- Questions and discussion

---

## Key features

- Continuous cluster scan — auto-discovers every dashboard, API, and internal tool
- Permanent front door — no more kubectl port-forward
- macOS Launchpad UX for Kubernetes apps
- Zeus AI — natural language Spotlight search and fleet health explanation
- Gateway to every workload with permanent URLs
- Annotation-aware discovery across all namespaces

---

## Installation

**Helm:**
```bash
helm repo add hypersdk https://charts.hypersdk.dev
helm install hermes hypersdk/hermes \
  -n hermes-system --create-namespace \
  --set global.domain=your-cluster.local
```

**Remote k3s deploy:**
```bash
git clone https://github.com/hypersdk/hermes && cd hermes
./scripts/deploy-remote.sh HOST USER
```

After install, Hermes continuously scans your cluster and builds a living application catalog. Open the Launchpad UI at the configured domain.

**Requirements:** Kubernetes 1.28+, DNS or ingress configured for your domain

---

## Report a bug

[Open a Bug Report →](../../issues/new?template=bug_report.yml)

Include: what you did, what happened, what you expected, your environment, and screenshots/logs (redact secrets).

## Request a feature

[Open a Feature Request →](../../issues/new?template=feature_request.yml)

## UX feedback

[Open a UX Feedback →](../../issues/new?template=ux_feedback.yml)

## Ask a question

Use [GitHub Discussions](../../discussions) for open-ended questions, ideas, and roadmap conversations.

---

## Security

**Do not report security vulnerabilities publicly.**

Email **security@zyvor.dev** — see [SECURITY.md](SECURITY.md).

---

## Do not post

- Source code or internal configuration
- API tokens, license keys, or credentials  
- Private logs with sensitive data
- Security vulnerabilities (email security@zyvor.dev)

---

Maintained by [Zyvor AI Labs](https://zyvor.dev)
