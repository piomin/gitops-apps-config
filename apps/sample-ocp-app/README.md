# Manifest Hydration

To hydrate the manifests in this repository, run the following commands:

```shell
git clone https://github.com/piomin/gitops-apps-config.git
# cd into the cloned directory
git checkout 1d06182211675912fe45857504a221d66bed3155
helm template . --name-template sample-ocp-app --namespace pminkows-test --values ./apps/sample-ocp-app/values-test.yaml --include-crds
```
