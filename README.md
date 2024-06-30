# Create Kubernetes config to launch Clickhouse & Superset pods in Minikube & connect them
## Kubernetes Deployment: Clickhouse and Superset on Minikube
This repository contains Kubernetes YAML configurations to deploy Clickhouse, an open-source data warehouse, and Superset, a business intelligence tool, on Minikube. Clickhouse is configured as a StatefulSet with persistent storage, while Superset is deployed as a Deployment. These configurations expose Clickhouse on port 9000 for Superset connectivity and Superset on port 8088 for web access.

## Key Files:

### clickhouse-statefulset.yaml: Defines Clickhouse deployment with persistent storage of 10GB.
### superset-deployment.yaml: Configures Superset deployment for creating reports and charts.
### clickhouse-service.yaml: Exposes Clickhouse service on port 9000.
### superset-service.yaml: Exposes Superset service on port 8088 (NodePort or LoadBalancer).

## Instructions:

### Deployment: Use kubectl apply -f <filename.yaml> to deploy these configurations on your Minikube cluster.
### Access: After deployment, access Superset via the exposed URL to connect and visualize data from Clickhouse.
