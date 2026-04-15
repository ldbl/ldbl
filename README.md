# ldbl

Production-first DevOps / SRE.

![Kubernetes](https://img.shields.io/badge/-Kubernetes-326CE5?logo=kubernetes&logoColor=white)
![FluxCD](https://img.shields.io/badge/-FluxCD-5468FF?logo=flux&logoColor=white)
![Terraform](https://img.shields.io/badge/-Terraform-7B42BC?logo=terraform&logoColor=white)
![Helm](https://img.shields.io/badge/-Helm-0F1689?logo=helm&logoColor=white)
![Kyverno](https://img.shields.io/badge/-Kyverno-1D63ED?logo=kyverno&logoColor=white)
![CloudNativePG](https://img.shields.io/badge/-CloudNativePG-336791?logo=postgresql&logoColor=white)
![Prometheus](https://img.shields.io/badge/-Prometheus-E6522C?logo=prometheus&logoColor=white)
![Grafana](https://img.shields.io/badge/-Grafana-F46800?logo=grafana&logoColor=white)
![Hetzner](https://img.shields.io/badge/-Hetzner-D50C2D?logo=hetzner&logoColor=white)
![Cloudflare](https://img.shields.io/badge/-Cloudflare-F38020?logo=cloudflare&logoColor=white)
![Go](https://img.shields.io/badge/-Go-00ADD8?logo=go&logoColor=white)
![Vue.js](https://img.shields.io/badge/-Vue.js-4FC08D?logo=vue.js&logoColor=white)

I build and document practical systems around:

- Kubernetes
- Terraform
- GitOps
- CI/CD guardrails
- observability
- backup / restore
- safe AI-assisted operations

## What I care about

I prefer:

- structure over confidence
- guardrails over improvisation
- rollback over clever fixes
- evidence over assumptions
- production safety over hype

## Current focus

I’m working on **SafeOps** — a guardrails-first approach to DevOps and SRE.

The goal is simple:

Build platforms that are safe to change, easy to reason about, and easier to recover when things go wrong.

## Featured projects

- **[sre](https://github.com/ldbl/sre)** — guardrails-first SRE control plane. Hetzner k3s + FluxCD + Terraform + Kyverno + CNPG, with SOPS/AGE secrets and default-deny networking.
- **[sre-course](https://github.com/safeops-course/sre-course)** — SafeOps course site (Hugo). 17 chapters mapped file-by-file to the `sre` implementation.
- **backend / frontend** — Go API and Vue 3 dashboard with health probes, Prometheus metrics, OpenTelemetry traces, and chaos endpoints.
- **k8s-ai-monitor** — Kopf-based Kubernetes operator with LLM-powered root-cause analysis.

## Principles I build by

**KISS, with humility.** No hieroglyphs. If you need a decoder ring to read it, rewrite it simpler.

- Explicit over implicit — clear names, documented intent
- Errors should never pass silently — fail loud, fail early
- In the face of ambiguity, refuse to guess — test and verify
- If it’s hard to explain, it’s a bad idea
- One obvious way to do it — establish patterns, stick to them
- Be humble enough to build systems better than yourself — safeguards that survive human error, context loss, and AI session resets

## Safety rails I don’t skip

- No direct commits to `main` — always a PR, always a review
- No `terraform apply` / `destroy` without explicit approval
- No secrets in git — SOPS + AGE, per-directory rules
- No amending pushed commits
- `default-deny` networking — new services declare their ingress/egress

## Mental model

AI is a very well-read junior engineer.

Useful.
Fast.
Confident.

But production still needs human judgment, review, and accountability.

## Elsewhere

- Website: https://safeops.work
- Course repo: https://github.com/safeops-course/sre-course
