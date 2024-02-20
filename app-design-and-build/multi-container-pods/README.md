- [The Distributed System ToolKit: Patterns for Composite Containers](https://kubernetes.io/blog/2015/06/the-distributed-system-toolkit-patterns/)
- [Pods resource sharing and communication](https://kubernetes.io/docs/concepts/workloads/pods/#resource-sharing-and-communication)
- [Shared Volumes](https://kubernetes.io/docs/tasks/access-application-cluster/communicate-containers-same-pod-shared-volume/)

Multi-container Patterns
- [Side Car Container](https://kubernetes.io/docs/concepts/workloads/pods/sidecar-containers/): performs a task that helps the main container 
- Ambassador Container: proxies container traffic 
- Adapter Container: transforms container output
- [Init Containers](https://kubernetes.io/docs/concepts/workloads/pods/init-containers/): specialized container that runs before the app container
    - delay startup
    - security
    
