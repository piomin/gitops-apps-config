# Manifest Hydration

To hydrate the manifests in this repository, run the following commands:

```shell
git clone https://github.com/piomin/gitops-apps-config.git
# cd into the cloned directory
git checkout 6c0689d5cc3d702317bad9a5166a52ca148edd18
helm template . --name-template sample-ocp-app --namespace pminkows-test --values ./apps/sample-ocp-app/values-test.yaml --include-crds
```
