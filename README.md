# Kubernetes Metrics Server

If you can see this, current branch is **camp-master**.

Some manifests were modified for the production environnment of wide-camp-1909.
Please refer to [master](https://github.com/wide-camp-1909/metrics-server/tree/master) branch and check the details.

## Getting Started
To use Horizontal Pod Autoscaling, you need to deploy this metrics-server in namespace kube-system first.
Run the following for installation and confirmation:

```
% kubectl apply -f deploy/1.8+/
% kubectl describe deployment metrics-server -n kube-system
% kubectl top nodes
```
