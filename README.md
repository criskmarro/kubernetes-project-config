# The Project configuration

This repository contains the Kubernetes manifests for The Project. Argo CD watches the `main` branch and synchronizes its root Kustomization to the `project` namespace.

The application source code is maintained in `KubernetesSubmissions`. Its GitHub Actions workflow publishes images and updates the image tags in this repository.

Bootstrap the Argo CD application once with:

```bash
kubectl apply -f argocd/the-project-application.yaml
```
