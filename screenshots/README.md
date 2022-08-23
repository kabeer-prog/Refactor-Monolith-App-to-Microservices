# Screenshots
To help review your infrastructure, please include the following screenshots in this directory::

## Deployment Pipeline
* DockerHub showing containers that you have pushed
* GitHub repository’s settings showing your Travis webhook (can be found in Settings - Webhook)
* Travis CI showing a successful build and deploy job

## Kubernetes
* To verify Kubernetes pods are deployed properly
```bash
kubectl get pods
```

![image](https://user-images.githubusercontent.com/77249754/186168850-e89581ec-eb38-4146-8611-e2528ccee561.png)

![image](https://user-images.githubusercontent.com/77249754/186169131-5c3169f0-6325-4665-a0d9-b09b7a611a0e.png)
* To verify Kubernetes services are properly set up
```bash
kubectl describe services
```
![image](https://user-images.githubusercontent.com/77249754/186172548-b711fd69-da24-40cb-bed6-1d39d8afcae8.png)
![image](https://user-images.githubusercontent.com/77249754/186172639-6ef0650d-ccd5-4a85-a3dc-bc1472667a14.png)
![image](https://user-images.githubusercontent.com/77249754/186172748-bda14573-1654-4793-a1d7-5f8737ce448c.png)
![image](https://user-images.githubusercontent.com/77249754/186172923-83f5cab8-cd4b-4f63-a340-4ec2ce8faba2.png)

* To verify that you have horizontal scaling set against CPU usage
```bash
kubectl describe hpa
```
![image](https://user-images.githubusercontent.com/77249754/186186025-0023a049-b36c-4ff0-ad4c-7d3395be6559.png)

* To verify that you have set up logging with a backend application
```bash
kubectl logs {pod_name}
```
