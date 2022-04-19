# Cluster

## :open_file_folder: Repository structure

This Git Repository contains the following directories and are ordered below by how Flux will apply them:

- **core** directory is where Flux deployments are located
- **crds** directory (depends on **core**) contains CustomResourceDefinitions that need to exist before anything else
- **infra** directory (depends on **crds**) contains infrastructure applications such as Traefik, MetalLB and so on
- **base** directory (depends on **infra**) contains applications that are useful for cluster operations such as K8up and so on
- **apps** directory (depends on **base**) is where common applications are located

```
./cluster
├── ./apps
├── ./base
├── ./core
├── ./crds
└── ./infra
```

---