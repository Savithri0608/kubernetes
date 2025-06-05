# Kubernetes Pod Deployment Example

This project demonstrates how to create and deploy a basic Kubernetes Pod using a declarative YAML configuration. It serves as a beginner-friendly entry into Kubernetes resource management and container orchestration.

![Deployment Screenshot](https://github.com/user-attachments/assets/10951f8f-fae5-4991-98f8-bbb8e84bc29f)

---

## 📌 Objective

Deploy a simple `nginx` container as a Kubernetes Pod using `kubectl` and understand the basic structure of Kubernetes YAML files.

---

## 🧱 YAML Configuration

Here is the basic pod configuration used:

```yaml
apiVersion: v1
kind: Pod
metadata:
  name: my-pod
spec:
  containers:
    - name: my-container
      image: nginx
      ports:
        - containerPort: 80
