# helm-python-web-app
helm-python-web-app

This a helm chart for a python web application
Deployment specs:
1. All configuration either in environment or ConfigMap 
2. CPU request/limit : 50m/150m
3. Memory request/limit : 80M/128M
4. Node Affinity:
- app-deployment = true
- db-deployment = false
- monitoring-deployment = false
5. App update strategy: Rolling update 
6. Specify HPA/HA and PDB for the pod
- HA/HPA : min/max 5/10
- PDB: 2
7. Enable and specify health check
8. All configuration to be used from 'values.yml' file.
