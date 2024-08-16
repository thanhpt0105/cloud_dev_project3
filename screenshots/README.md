# Screenshots
To help review your infrastructure, please include the following screenshots in this directory::

## Deployment Pipeline
* DockerHub showing containers that you have pushed
```
docker_hub_images.png
```

* GitHub repository’s settings showing your Travis webhook (can be found in Settings - Webhook)

**Using Github Action instead of Travis for CI**
```
github_actions.png
```
* Github action show successfully build and push images to docker hub
```
github_action_01.png
github_action_02.png
github_action_03.png
github_action_04.png
```

## Kubernetes
* To verify Kubernetes pods are deployed properly
```bash
kubectl get pods
```
Screenshot:
```
kubectl_get_pods.png
```
* To verify Kubernetes services are properly set up
```bash
kubectl describe services
```
Output:
```
describe_services.txt
```
* To verify that you have horizontal scaling set against CPU usage
```bash
kubectl describe hpa
```
Output:
```
describe_hpa.txt
```
**Submit 2:**
```
kubectl_hpa.png
```
* To verify that you have set up logging with a backend application
```bash
kubectl logs {pod_name}
```
Screenshot:
```
kubectl_logs.png
```
**Submit 2:**
```
kubectl_logs_with_api_call.png
```

* App URL:
```
http://aa9ac93cb349045478a69920741c0511-1086837889.us-east-1.elb.amazonaws.com/
```
