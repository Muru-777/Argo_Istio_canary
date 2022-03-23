# Argo_Istio_canary

This repository helps to deploy the code using canary deployment strategy.

Urls:

Canary:
https://dev.to/stack-labs/canary-deployment-with-argo-cd-and-istio-406d

To deploy istio: 
https://istio.io/latest/docs/setup/getting-started/#download

Blue green:
https://blog.baeke.info/2021/11/01/kubernetes-blue-green-deployments-with-argo-rollouts/

Canary:
https://particule.io/en/blog/argocd-canary/

while true; do curl -s $appname | jq .color; sleep 0.5; done

argocd https://argo-cd.readthedocs.io/en/stable/getting_started/

step 2: https://tanzu.vmware.com/developer/guides/argocd-gs/

argocd app create colorapi --repo https://github.com/kabilanmani93/canary.git --path . --dest-server https://kubernetes.default.svc --dest-namespace default

