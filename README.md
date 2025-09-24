# myapp-gitops
myapp-gitops

# Structure

    myapp-gitops/
    │
    ├── apps/                       # ArgoCD Applications definitions
    │   └── myapp.yaml
    │
    ├── base/                       # K8s manifests (common for all envs)
    │   ├── deployment.yaml
    │   ├── service.yaml
    │   └── namespace.yaml
    │
    ├── overlays/                   # Env-specific configs
    │   ├── dev/
    │   │   └── kustomization.yaml
    │   ├── staging/
    │   │   └── kustomization.yaml
    │   └── prod/
    │       └── kustomization.yaml
    │
    └── README.md
