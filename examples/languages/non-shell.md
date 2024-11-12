## Non-Shell Languages

You can use the `interpreter` annotation to use different programming languages or to visualize files in different formats, like YAML. In this example the interpreter is set to 'cat'.

Take a look at the following YAML file for creating a Kubernetes Deployment object:

```yaml {"id":"01HTZB059ZFK301922YJXQTM2D","interpreter":"cat"}
apiVersion: apps/v1
kind: Deployment
metadata:
  name: nginx-deployment
  labels:
    app: nginx
spec:
  replicas: 3
  selector:
    matchLabels:
      app: nginx
  template:
    metadata:
      labels:
        app: nginx
    spec:
      containers:
        - name: nginx
          image: nginx:latest
          ports:
            - containerPort: 80
```
