## Create ReplicationController
```
kubectl run kubia --image=mantissaman/ckd-kubia --port=8080 --generator=run/v1
```

## Expose ReplicationController to LoadBalancer
```
kubectl expose rc kubia --type=LoadBalancer --name kubi-http
```

## Scale ReplicationController
```
kubectl scale rc kubia --replicas=3
```

