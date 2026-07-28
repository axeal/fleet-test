```
kind: GitRepo
apiVersion: fleet.cattle.io/v1alpha1
metadata:
  name: test
  namespace: fleet-local
spec:
  repo: https://github.com/axeal/fleet-test.git
  branch: "01886042"
  paths:
  - Elemental/CRDs
  - Elemental/Operator
  targets:
   # Match everything
  - clusterSelector: {}
```
