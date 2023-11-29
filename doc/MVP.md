# Demonstration of the operation of the ambassador project deployed in the local kubernetes k3d cluster

## Commands: 

The kubectl get all command is used to retrieve information about resources in a Kubernetes cluster. The -n flag is used to specify the namespace for which you want to get information. In your case, it's set to demo.

Here's a breakdown of the command:

```
kubectl get all -n demo
```
* kubectl: The command-line tool for interacting with Kubernetes clusters.
* get: Retrieves one or more resources.
* all: Specifies that information about all resource types should be retrieved.
* -n demo: Sets the namespace to "demo," meaning the command will retrieve information only for resources in the "demo" namespace.
T
his command will display information about various resources (pods, services, deployments, etc.) within the specified namespace (demo). Keep in mind that not all resource types support the all keyword. In some cases, you might need to specify the resource type explicitly.


```
kubectl get all -n demo

```

The kubectl get po command is used to retrieve information about pods in a Kubernetes cluster. The -n flag is used to specify the namespace for which you want to get information. In your case, it's set to demo.

Here's a breakdown of the command:

```
kubectl get po -n demo
```

* kubectl: The command-line tool for interacting with Kubernetes clusters.
* get: Retrieves one or more resources.
* po: Specifies that information about pods should be retrieved.
* -n demo: Sets the namespace to "demo," meaning the command will retrieve information only for pods in the "demo" namespace.
This command will display a list of pods in the "demo" namespace, including their names, status, and other relevant information. It's a quick way to check the status of pods within a specific namespace.

```
kubectl get po -n demo
```

Getting the ambasador app version
```
curl localhost:8088
```

Downloading image

```
wget -O https://www.nicepng.com/png/full/2-28004_images-branding-googlelogo-2x-googlelogo-color-272x92dp-custom.png
```


curl -F 'image=@tmp/name.png' localhost:8088/img/


