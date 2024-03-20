[Volumes](https://kubernetes.io/docs/concepts/storage/volumes/)

- [hostPath](https://kubernetes.io/docs/concepts/storage/volumes/#hostpath): data stored on host file system
- [emptyDir](https://kubernetes.io/docs/concepts/storage/volumes/#emptydir): data stored in managed location; deleted if Pod is deleted
- [persistentVolume](https://kubernetes.io/docs/concepts/storage/persistent-volumes/): abstracts storage resource (points to underlying storage resource)
- [persistentVolumeClaim](https://kubernetes.io/docs/concepts/storage/volumes/#persistentvolumeclaim): data stored using a persistent volume (a request for storage needed => binds to persistent volume)

- `spec.volumes` defines volumes in the Pod
- `spec.containers.volumeMounts` attaches pod volumes to the container at a specific location