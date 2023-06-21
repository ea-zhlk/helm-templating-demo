# Overview

To see the templated YAML files run the following with the corresponding values.yaml file:

```bash
helm template . --values values-dev.yaml
```

To install the helm chart into the kubernetes cluster, run the following command:

```bash
helm install test-app . --values=values-dev.yaml 
```

To see the actual manifests that was deployed, run the following command:

```bash
helm get manifest test-app
```

You can upgrade your helm chart:

```bash
 helm upgrade test-app . --values=values-dev.yaml
```

To uninstall the deployed helm chart:

```bash
helm uninstall test-app
```
