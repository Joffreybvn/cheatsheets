## Basics

By default, `kubectl get pods` list all pods in the default namespace. Which is empty.

### Namespaces and Pods

- To get detailed infos, add `-o wide` to the command's parameters

#### Creating a namespace
Create a namspace in order to instantiate services in it later
```shell
kubectl create namespace <namespace>
```

#### Listing all namespaces
List all kubernetes namespaces
```shell
kubectl get ns
```

#### Listing all pods of all namespaces
List all pods accross all namespaces
```shell
kubectl get pods -A
```

#### Listing pods in a namespace
```shell
kubectl get pods -n <namespace>
```

### ConfigMaps

#### Listing ConfigMaps in a namespace
```shell
kubectl get configmaps -n <namespace>
```
