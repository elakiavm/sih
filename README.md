```
kind load docker-image fe --name chat-k8s
kind load docker-image be --name chat-k8s

```

```
kubectl apply -f k8s/
```

```
kubectl port-forward svc/chat-fe 3000:3000
kubectl port-forward svc/chat-be 3001:3001

```

https://kubernetes.io/docs/tasks/tools/install-kubectl-linux/