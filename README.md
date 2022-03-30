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

## Block bad IP

Add ip threat feed in calico
```
kubectl apply -f https://raw.githubusercontent.com/JeremyTigera/Kubernetes-Security-Workshop/main/IPS-feed/threat-feed.yaml
```

## Secure nodes by adding label to make then endpoint

## Securing EKS hosts:

Automatically register your nodes as Host Endpoints (HEPS). To enable automatic host endpoints, edit the default KubeControllersConfiguration instance, and set ``` spec.controllers.node.hostEndpoint.autoCreate```  to ```true``` for those ```HostEndpoints``` :

```
kubectl patch kubecontrollersconfiguration default --patch='{"spec": {"controllers": {"node": {"hostEndpoint": {"autoCreate": "Enabled"}}}}}'
```
