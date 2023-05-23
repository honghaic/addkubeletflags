# Add the kubelet flags - CPU Manager Policy and Topology Manager Policy

### This will allow you to change the CPU Manager and Topology Manager policies to "static" and "best-effort" respectively to *all the nodes* in an existing AKS cluster

Run the following commands to apply the changes on all the nodes.

```sh
kubectl apply -f https://raw.githubusercontent.com/dqmicrosoft/addkubeletflags/main/addkubeletflags.yaml
sleep 5
kubectl delete -f https://raw.githubusercontent.com/dqmicrosoft/addkubeletflags/main/addkubeletflags.yaml
```
