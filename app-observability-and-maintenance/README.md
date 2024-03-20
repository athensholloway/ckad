Observability and Maintanance


- API Deprecation Policy
    - Annoucing changes to the API early
    - Deprecated API in GA (Generally Availabe) removed after 12 months or 3 Kubernetes releases
      - Deprication window: GA 3 release or 12 Month, Beta 2 release or 9 Month, Alpha...
    - `apiVersion` indicates which version the yml is compatible with
- Probes and Health Checks: healthc status monitoring
    - liveness: check if container is healthy or needs to be restrated
    - readiness: determines when the container is started and ready
    - startup: checks health during startup; check for slow starting containers
- Monitoring: container status and performance
- Container Logging: accessing log container output
- Debugging: troubleshooting kubernetes applications
