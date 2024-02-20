Setup a local multi-node Kubernetes cluster w/ [KinD](https://kind.sigs.k8s.io).

`brew install kind`



 Configure the [extraPortMappings](https://kind.sigs.k8s.io/docs/user/configuration/#extra-port-mappings) setting in `kind.yml` for port forwarding to KinD nodes.

 `kind create cluster --config=kind.yml`

 `kind get clusters`

 `kubectl get nodes`