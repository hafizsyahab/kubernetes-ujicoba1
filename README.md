# Kubernetes Local Practice (kind)
🚧 **Status: Ongoing** — currently learning Kubernetes Autoscaling (HPA), next: Terraform + AWS.

## ⚠️ Note on Secrets
All values in `secret.yaml` (e.g. `PASSWORD_CONTOH`) are dummy/placeholder data created solely for demonstrating Kubernetes Secret concepts. No real credentials or third-party data are used in this project.

## About
Personal learning project to practice core Kubernetes concepts using a local
cluster (`kind`, running via Docker Desktop). This is not a production
deployment — it's a hands-on sandbox to understand how each Kubernetes
resource works.

## What's covered
- Control Plane, Pods, and basic cluster architecture
- Deployments & ReplicaSets
- Services
- Namespaces
- ConfigMaps & Secrets
- Persistent Volumes & Persistent Volume Claims
- Health check probes (liveness/readiness)
- Ingress (Ingress Controller + routing via `kubectl port-forward`)
- A basic CI/CD-oriented deployment file (`deployment-cicd.yaml`)

## Files
| File | Purpose |
|---|---|
| `deployment.yaml` | Basic Deployment example |
| `service.yaml` | Exposing a Deployment via Service |
| `configmap.yaml` | Injecting config data into Pods |
| `secret.yaml` | Injecting sensitive data into Pods |
| `pv.yaml` / `pvc.yaml` | Persistent storage setup |
| `real-app.yaml` | Small sample app tying concepts together |
| `pod-configmap.yaml` | Pod consuming a ConfigMap |
| `pod-with-pvc.yaml` | Pod consuming a Persistent Volume Claim |
| `deployment-cicd.yaml` | Deployment used for CI/CD pipeline practice |

## Environment
- Local Kubernetes cluster via `kind`, run through Docker Desktop
- `kubectl` for cluster management

## Next steps
- Horizontal Pod Autoscaling (HPA)
- Terraform + AWS
- Serverless (Lambda) & event-driven patterns (SQS)