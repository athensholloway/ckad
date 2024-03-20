Setup a local multi-node Kubernetes cluster w/ [KinD](https://kind.sigs.k8s.io).

`brew install kind`



 Configure the [extraPortMappings](https://kind.sigs.k8s.io/docs/user/configuration/#extra-port-mappings) setting in `kind.yml` for port forwarding to KinD nodes.

 `kind create cluster --config=kind.yml`

 `kind get clusters`

 `kubectl get nodes`


`kubectl config set-context --current --namespace <namespace>`

[Debugging Kubernetes Nodes With Kubectl](https://kubernetes.io/docs/tasks/debug/debug-cluster/kubectl-node-debug/)
[Shell access to node or pod](https://medium.com/@the_good_guy/get-shell-access-to-pods-nodes-in-kubernetes-using-kubectl-1d8fc10e89eb)
[Shell access to KinD worker node](https://stackoverflow.com/questions/69108075/how-to-ssh-into-kind-cluster-nodes-with-containerd-runtime) requires `docker exec -it [worker node] sh`

 Exam Resources:
 - https://medium.com/@michael_england/how-i-passed-the-certified-kubernetes-application-developer-ckad-exam-cd443f160643#:~:text=This%20means%20that%20it%20is,for%20the%20exam%20is%2066%25.
 - https://killercoda.com/killer-shell-ckad
 - https://www.youtube.com/watch?v=wHha-Q3XVOg