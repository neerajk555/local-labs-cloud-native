# Local Docker & Kubernetes Fundamentals Labs

Non-AWS track. Runs entirely on your own machine — no AWS account, no
cost, no `$PARTICIPANT` variable needed, since there's nothing shared
here. Sibling to `../aws-cloudnative-agentic-ai-labs/`, never modifies it.

**Recommended:** do Module L3 (Kubernetes Fundamentals with `kind`)
before the AWS repo's Module 4 (EKS) if you haven't used Kubernetes
before — the concepts (Deployments, Services, namespaces, rolling
updates) are identical; EKS just adds AWS-specific plumbing on top.

## Prerequisites

- Docker Desktop
- `kind` (`go install sigs.k8s.io/kind@latest` or via package manager)
- `kubectl`
- `helm` (Module L5 only)

## Modules

| Module | Topic |
|---|---|
| L1 | Docker Fundamentals Deep-Dive |
| L2 | Docker Compose |
| L3 | Kubernetes Fundamentals with `kind` |
| L4 | Kubernetes Workloads & Storage |
| L5 | Helm: Authoring Your Own Chart |
| L6 | Ingress (ingress-nginx) |
