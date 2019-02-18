K8s Shell Demo (Clear Linux based)
=======
This provides a shell demo by deploying nginx on Clear Linux* based container OS.
Google provide shell demo registry at https://k8s.io/examples/application/shell-demo.yaml which using default nginx docker containter from https://hub.docker.com/_/nginx which based on Debian as container OS.

The de
Create the Pod
-----
```
kubectl create -f https://raw.githubusercontent.com/kenplusplus/clear-k8s-registries/master/clr-shell-demo/clr-shell-demo.yaml
```

Verify that the Container is running
---------------------------
```
kubectl get pod clr-shell-demo
```

Get a shell to the running Container
-----------------------
```
kubectl exec -it clr-shell-demo -- /bin/bash
```