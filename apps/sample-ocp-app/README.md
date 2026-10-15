# Manifest Hydration

To hydrate the manifests in this repository, run the following commands:

```shell
git clone https://github.com/piomin/gitops-apps-config.git
# cd into the cloned directory
git checkout 6c162a6edb67a36de254ca2736daf40a7c2c01a4
helm template . --name-template sample-ocp-app --namespace pminkows-dev --values ./apps/sample-ocp-app/values-dev.yaml --include-crds
```
