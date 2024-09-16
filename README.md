# rhdh-gke

Directory Structure

```
── payment-catalog-repo
│   └── catalog-entities
│       ├── all.yaml
│       ├── apis
│       │   └── payments.yaml
│       ├── components
│       │   └── backend.yaml
│       ├── docs
│       │   └── index.md
│       ├── resources
│       │   └── pg-database.yaml
│       └── systems
│           └── payment.yaml
└── rhdh-pe
    ├── app-config
    │   ├── app-config-prod.yaml
    │   └── app-config-test.yaml
    ├── plugins
    │   └── fluxcd
    ├── templates
    ├── values-test.yaml
    └── values.yaml
```

Helm Repo

```
helm repo add openshift-helm-charts-ci-1.3 https://github.com/rhdh-bot/openshift-helm-charts/raw/redhat-developer-hub-1.3-84-CI/installation
helm repo update openshift-helm-charts-ci-1.3
helm search repo openshift-helm-charts-ci-1.3 --devel
helm template rhdh openshift-helm-charts-ci-1.3/redhat-developer-hub --devel
```

