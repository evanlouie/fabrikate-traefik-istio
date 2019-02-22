# Fabrikate-Traefik-Istio

> A Fabrikate definition to use Traefik as your exposed LB and route all traffic into an Istio service mesh

- Istio will be installed to namespace `istio-system`
- Traefik will be installed to namespace `traefik`
- Istio's `istio-ingressgateway` will now be of of type `ClusterIP` (no longer a `LoadBalancer`)
- This component will provision a Traefik ingress in the `istio-system` namespace and proxy all traffic to `istio-ingressgateway`
