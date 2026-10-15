# Manifest Hydration

To hydrate the manifests in this repository, run the following commands:

```shell
git clone https://github.com/piomin/gitops-apps-config.git
# cd into the cloned directory
git checkout db7d33d2d21eff3689849a13081b64e39b223559
helm template . --name-template sample-ocp-app --namespace pminkows-dev --values ./apps/sample-ocp-app/values-dev.yaml --include-crds
```
