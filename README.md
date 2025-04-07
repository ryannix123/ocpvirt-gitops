# Fedora VM - GitOps Deployment with ArgoCD

This repo contains a VirtualMachine definition (KubeVirt) for deploying a Fedora-based VM on OpenShift via GitOps using ArgoCD.

## 🚀 Getting Started

1. Fork this repo to your GitHub account.
2. Update `argocd/application.yaml`:
   - Set `repoURL` to your GitHub repo URL.
3. Apply the ArgoCD application:

```bash
oc apply -f argocd/application.yaml
```

4. ArgoCD will deploy the VM into the `vm` namespace.

## 🔒 Credentials

- **Username**: `fedora`
- **Password**: `8x2f-8eok-4di0`

## 🧠 Notes

- Run strategy: `RerunOnFailure`
- Uses a DataVolume source named `fedora` from `openshift-virtualization-os-images`.
