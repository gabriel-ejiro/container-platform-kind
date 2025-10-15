# Container Platform (KIND + GitHub Actions)

**Goal:** simulate an EKS-style workflow at $0 cost using KIND in CI.

## What happens on every push
1. A KIND cluster starts inside the GitHub runner.  
2. `demo-web` (nginx) is deployed and rolled out.  
3. CI port-forwards and fetches the homepage (smoke test).  
4. Evidence (kubectl outputs + HTML) is published to GitHub Pages.

## This is important because
- **Infrastructure as code:** repeatable cluster bootstrapping.
- **Kubernetes skills:** manifests, rollouts, services, ingress.
- **CI discipline:** tests and artifacts that prove it’s working.

🔗 Demo evidence: (link to your Pages URL)
