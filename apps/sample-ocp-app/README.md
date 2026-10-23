# Manifest Hydration

To hydrate the manifests in this repository, run the following commands:

```shell
git clone https://github.com/piomin/gitops-apps-config.git
# cd into the cloned directory
git checkout 73b0c653d5858acc32a4d9c4c569db9893fd15e8
helm template . --name-template sample-ocp-app --namespace pminkows-test --values ./apps/sample-ocp-app/values-test.yaml --include-crds
```
