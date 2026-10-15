# Manifest Hydration

To hydrate the manifests in this repository, run the following commands:

```shell
git clone https://github.com/piomin/gitops-apps-config.git
# cd into the cloned directory
git checkout 0acef507df459339e60afc5996fc5f8642acd3c5
helm template . --name-template sample-ocp-app --namespace pminkows-prod --values ./apps/sample-ocp-app/values-prod.yaml --include-crds
```
