# argoroll-bg


```shell
kubectl create namespace argo-rollouts
kubectl get ns argo-rollouts
kubectl apply -n argo-rollouts -f https://github.com/argoproj/argo-rollouts/releases/latest/download/install.yaml
kubectl get all -n argo-rollouts
```

```shell
curl -LO https://github.com/argoproj/argo-rollouts/releases/latest/download/kubectl-argo-rollouts-linux-amd64
chmod +x ./kubectl-argo-rollouts-linux-amd64
sudo mv ./kubectl-argo-rollouts-linux-amd64 /usr/local/bin/kubectl-argo-rollouts
kubectl argo rollouts version
```

```shell
kubectl argo rollouts dashboard
```


```shell
kubectl argo rollouts get rollout rollout-bluegreen
kubectl argo rollouts set image rollout-bluegreen rollouts-demo=argoproj/rollouts-demo:green
kubectl argo rollouts get rollout rollout-bluegreen
kubectl argo rollouts promote rollout-bluegreen
kubectl argo rollouts get rollout rollout-bluegreen

```
