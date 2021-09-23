# Nginx-Ingress-Controller-Setup
Installation of Nginx ingress controller with Kustomize support

The idea is that we take the default Nginx-ingress-controller from https://kubernetes.github.io/ingress-nginx/deploy/#azure and edit it with Kustomize overlays. To install run:
````
> kubectl kustomize overlays/dev
````
Please edit the patch-ingress-controller.yaml to change where the cloud providers load balancers should be created.