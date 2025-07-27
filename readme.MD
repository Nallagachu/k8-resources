
# Kubernetes Resource Examples ☸️

This repository offers practical YAML manifest files to help you quickly grasp core Kubernetes concepts. It's designed for hands-on learning, showcasing essential resource types and their capabilities.

---

## 🚀 Why This Repo?

* **Quick Learning:** Understand Kubernetes fundamentals with clear, focused examples.
* **Core Concepts:** See how common resources work in practice.
* **Hands-on:** Easily apply and experiment with each file on your cluster.

---

## 📁 Resource Quick Guide

| File Name               | Resource Type         | What it Shows                                          |
| :---------------------- | :-------------------- | :------------------------------------------------------- |
| `01-namespace.yaml`     | **Namespace** | Isolating resources.                                     |
| `02-pod.yaml`           | **Pod** | The basic building block (single container).             |
| `03-multi-container.yaml` | **Pod** | Multi-container patterns (e.g., sidecars).               |
| `04-labels.yaml`        | **Labels** | Grouping and selecting objects.                          |
| `05-annotations.yaml`   | **Annotations** | Attaching non-identifying metadata.                      |
| `06-resources.yaml`     | **Resource Limits** | Managing CPU/memory.                                     |
| `07-env.yaml`           | **Environment Variables** | Injecting configuration.                                 |
| `08-config-map.yaml`    | **ConfigMap** | Externalizing configurations.                            |
| `09-pod-config.yaml`    | **Pod using ConfigMap** | Consuming ConfigMaps in pods.                            |
| `10-secret.yaml`        | **Secret** | Storing sensitive data securely.                         |
| `11-pod-secret.yaml`    | **Pod using Secret** | Utilizing Secrets in pods.                               |
| `12-service.yaml`       | **ClusterIP Service** | Exposing applications internally.                        |
| `13-service-np.yaml`    | **NodePort Service** | Exposing applications on node ports.                     |
| `14-service-lb.yaml`    | **LoadBalancer Service** | Exposing apps via cloud load balancers.                  |
| `15-replicaset.yaml`    | **ReplicaSet** | Ensuring a desired pod count.                            |
| `16-deployment.yaml`    | **Deployment** | Managing ReplicaSets and rolling updates.                |

---

## 👨‍💻 How To Use

You'll need `kubectl` configured with a Kubernetes cluster.

```bash
# Apply a file
kubectl apply -f <filename>.yaml

# Example
kubectl apply -f 02-pod.yaml

# Check resource status
kubectl get pod
kubectl describe pod <pod-name>
````

-----

## 💡 Learning Tips

  * Use `kubectl explain <resource>` for schema details.
  * Modify YAML files and reapply to see changes.
  * `kubectl describe` is great for debugging.

-----

## 📝 License

This repo is for educational use. Feel free to fork and contribute\!

Happy K8s Learning\! 🚀

```
```