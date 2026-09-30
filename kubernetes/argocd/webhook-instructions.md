# GitHub Webhook Setup for ArgoCD

## Get ArgoCD Webhook URL
```bash
# The webhook endpoint is:
https://argocd.arkhaya.duckdns.org/api/webhook
```

## GitHub Setup
1. Go to your repo: https://github.com/GauranshMathur/Homelab
2. Settings → Webhooks → Add webhook
3. Payload URL: `https://argocd.arkhaya.duckdns.org/api/webhook`
4. Content type: `application/json`
5. Secret: (leave empty for now)
6. Events: Just the push event
7. Active: ✓

## Benefits
- Instant sync on git push
- No 3-minute wait
- More responsive GitOps