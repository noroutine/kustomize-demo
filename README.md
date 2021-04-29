With [kustomize](https://kustomize.io/) ([docs](https://github.com/kubernetes-sigs/kustomize/blob/master/cmd/config/docs/commands/create-setter.md))
```bash
# in any yaml folder
kustomize cfg init .
kustomize cfg create-setter . version v0.1
kustomize cfg set . version v0.2
```

With [yq](https://mikefarah.gitbook.io/yq) ([docs](https://mikefarah.gitbook.io/yq/v/v4.x/upgrading-from-v3#updating-writing-documents))
```bash
yq eval '.top[0].version = "v0.3"' test.yml
```
