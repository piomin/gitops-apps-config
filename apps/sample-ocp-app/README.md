# Manifest Hydration

To hydrate the manifests in this repository, run the following commands:

```shell
git clone https://github.com/piomin/gitops-apps-config.git
# cd into the cloned directory
git checkout 8e973d99d613a9fb1f597324c5170719c6c99596
helm template . --name-template sample-ocp-app --namespace pminkows-prod --values ./apps/sample-ocp-app/values-prod.yaml --include-crds
```
