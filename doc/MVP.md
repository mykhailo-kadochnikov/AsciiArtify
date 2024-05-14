# Port Forwarding to Access ArgoCD
```bash
kubectl port-forward svc/argocd-server -n argocd 8080:443
# argocd admin initial-password -n argocd
```bash
argocd admin initial-password -n argocd
# Logging into ArgoCD Dashboard via CLI
```bash
argocd login localhost:8080
# Logging into ArgoCD Dashboard via GUI
# Creating app via GUI
# Syncing app via GUI
# Creating app via CLI
```bash
argocd app create mvp2 --repo https://github.com/den-vasyliev/go-demo-app --path helm --dest-server https://kubernetes.default.svc --dest-namespace default
# Syncing app via CLI
```bash
argocd app sync mvp2
#Record of executing task
https://drive.google.com/file/d/1Qn9bVN3hdAIVIAsf5fpD4vzCyZ03vwiW/view?usp=sharing
