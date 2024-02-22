[Deployents](https://kubernetes.io/docs/concepts/workloads/controllers/deployment/) define a desired state for replica pods. manages replica pods using a pod template. Allows scaling up or down.

- Rolling Updates
- Deployment Strategies
- Helm Package Manager

[Updating Deployments](https://kubernetes.io/docs/concepts/workloads/controllers/deployment/#updating-a-deployment)
- Rolling Updates: change a deployments pod templates with zero downtime

- Rollout are triggered by changes to the deployments pod template e.g. `.spec.template` 
- Use `kubectl rollout status deployment/<$DeploymentName>` to check the status of the rollout 
- Rollback the latest rolling update with `kubectl rollout undo deployment/<$DeploymentName>`


Deployment Strategy
 - Blue/Green - 2 identical production environment. users currently use blue environment. roll out to green then cut over
 - Canary - second environment and a small portion of userbase uses the canary environmet.