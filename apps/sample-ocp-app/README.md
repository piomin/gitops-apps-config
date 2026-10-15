# Manifest Hydration

To hydrate the manifests in this repository, run the following commands:

```shell
git clone https://github.com/piomin/gitops-apps-config.git
# cd into the cloned directory
git checkout 51e4953f0d273888c33eb77280d337aaee03267a
helm template . --name-template sample-ocp-app --namespace pminkows-prod --values ./apps/sample-ocp-app/values-prod.yaml --include-crds
```
