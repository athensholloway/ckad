[Volumes](https://kubernetes.io/docs/concepts/storage/volumes/)

- [hostPath](https://kubernetes.io/docs/concepts/storage/volumes/#hostpath): data stored on host file system
- [emptyDir](https://kubernetes.io/docs/concepts/storage/volumes/#emptydir): data stored in managed location; deleted if Pod is deleted
- [persistentVolume](https://kubernetes.io/docs/concepts/storage/persistent-volumes/): abstracts storage resource (points to underlying storage resource)
- [persistentVolumeClaim](https://kubernetes.io/docs/concepts/storage/volumes/#persistentvolumeclaim): data stored using a persistent volume (a request for storage needed => binds to persistent volume)


[Debugging Kubernetes Nodes With Kubectl](https://kubernetes.io/docs/tasks/debug/debug-cluster/kubectl-node-debug/)
[Shell access to node or pod](https://medium.com/@the_good_guy/get-shell-access-to-pods-nodes-in-kubernetes-using-kubectl-1d8fc10e89eb)
[Shell access to KinD worker node](https://stackoverflow.com/questions/69108075/how-to-ssh-into-kind-cluster-nodes-with-containerd-runtime) requires `docker exec -it [worker node] sh`

- `spec.volumes` defines volumes in the Pod
- `spec.containers.volumeMounts` attaches pod volumes to the container at a specific location