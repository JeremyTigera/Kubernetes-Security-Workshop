# Kubernetes-Security-Workshop

bla bla summury best secu kub practices

## Install app

If your cluster does not have applications, you can use the following storefront application:
```
kubectl apply -f https://installer.calicocloud.io/storefront-demo.yaml
```

Confirm it is deployed, get pod storefront blabla commands

```
kubectl get pods -n storefront --show-labels
```

Create tier blabla
```
kubectl apply -f https://raw.githubusercontent.com/JeremyTigera/Kubernetes-Security-Workshop/main/policies/app-tier.yaml
```

**INSERT SCREENSHOT**

