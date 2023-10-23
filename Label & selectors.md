# Label selectors
vi label.yml
```bash
apiVersion: v1
kind: Pod
metadata:
  name: label-demo
  labels:
    environment: production
    app: nginx
spec:
  containers:
  - name: nginx
    image: nginx:1.14.2
    ports:
    - containerPort: 80
```
- Labe : Define , apply label on node, pod, object
- Selector : Select labeled pods, objects

```bash
kubectl apply -f label.yml

```











