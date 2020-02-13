# Cheat Sheet for Istioctl (and Istio in general)

Verify Istio install 
`istioctl verify-install`

Look at all proxies status 
`istioctl proxy-status`

Check TLS for foo pod in default namespace  
`istioctl authn tls-check foo-656bd7df7c-5zp4s.default`

Open Istio dashboard  
`istioctl dashboard grafana`

Open Pilot Dashboard 
`istioctl dashboard controlz $(kubectl get pod -n istio-system -l app=pilot -o jsonpath='{..metadata.name}').istio-system`

