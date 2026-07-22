```
kind: GitRepo
apiVersion: fleet.cattle.io/v1alpha1
metadata:
  name: test
  namespace: fleet-default
spec:
  repo: https://github.com/axeal/fleet-test.git
  branch: 01846429-kustomize
  targets:
  - name: custom
    clusterSelector:
      matchLabels:
        env: custom
  - name: do
    clusterSelector:
      matchLabels:
        env: do
```
