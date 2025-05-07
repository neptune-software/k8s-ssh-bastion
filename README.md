# k8s-ssh-bastion

```
helm install k8s-bastion oci://ghcr.io/neptune-software/charts/k8s-ssh-bastion
```

It just runs several sshd pods with NodePort and allows users to authenticate by ssh public key. Autocreated secrets are used to store server keys.
