# Manifest Hydration

To hydrate the manifests in this repository, run the following commands:

```shell
git clone https://github.com/piomin/gitops-apps-config.git
# cd into the cloned directory
git checkout a37a1c269eea93b9d1bc6cec6270185a2aecdea1
helm template . --name-template sample-ocp-app --namespace pminkows-prod --values ./apps/sample-ocp-app/values-prod.yaml --include-crds
```
