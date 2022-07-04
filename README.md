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




===============
Argo canary with istio:

https://dev.to/stack-labs/canary-deployment-with-argo-cd-and-istio-406d

https://confluence.fkinternal.com/display/CBS/CD+Onboarding+Guidelines 

https://github.fkinternal.com/Flipkart/fk-build-flow-demo/blob/master/charts/values.yaml 


https://particule.io/en/blog/argocd-canary/\

Kabilan M11:33 AM
 kubectl port-forward svc/argocd-server -n argocd 8080:443
Kabilan M11:34 AM
aX-aH42lxVZX-n9a
Kabilan M11:37 AM
https://argo-cd.readthedocs.io/en/stable/getting_started/
Kabilan M11:45 AM
argocd app create colorapi --repo https://github.com/kabilanmani93/canary.git --path . --dest-server https://kubernetes.default.svc --dest-namespace default
Kabilan M11:53 AM
argocd repo add git@github.com:argoproj/argocd-example-apps.git --ssh-private-key-path ~/.ssh/id_rsa


https://medium.com/@Oskarr3/setting-up-ingress-on-minikube-6ae825e98f82

while true; do curl http://127.0.0.1:8001/api/v1/namespaces/default/services/colorapi:http/proxy/ | jq .color; sleep 0.5; done
http://127.0.0.1:8001/api/v1/namespaces/default/services/colorapi:http/proxy/

https://argoproj.github.io/argo-rollouts/features/traffic-management/istio/

minikube start  --extra-config=apiserver.enable-swagger-ui=true

http://127.0.0.1:8001/api/v1/namespaces/default/services/colorapi:http/proxy/
