# Prometheus and Grafana applications deployment to Kubernetes

These resources will be created:

* Prometheus Persistent Volume Claim
* Prometheus ConfigMap
* Prometheus Deployment
* Prometheus Service
* Prometheus Datasource

---

* Grafana Persistent Volume Claim
* Grafana Credentials
* Grafana ConfigMap
* Grafana Deployment
* Grafana Service


## To run this flow in Minikube, you will need to have Minikube installed and running. Here are the steps to follow:

- Start Minikube:
`minikube start`
- Create Prometheus and Grafana resources
`kubectl apply -f .`
- Once all the resources are created, you can access Grafana by getting the IP address of the Minikube cluster and the port number of the Grafana service:
`minikube service grafana-service --url`

This command will return the URL that you can use to access Grafana, which should be in the format **http://<IP_ADDRESS>:<PORT_NUMBER>**. Open this URL in your web browser, and you should see the Grafana login page. Use the username and password specified in the `grafana-credentials.yaml` file to log in.

