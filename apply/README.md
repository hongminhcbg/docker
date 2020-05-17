$ kubectl apply -f filename.yaml
yaml better for human
json better for computer

- Each file contains one or more manifests
- Each manifests describe an API objects (deployment, job, secret)
- Each manifest needs four part
    - apiVersion
    - kind
    - metadata
    - spec

- kind
    - $ kubectl api-resources # show all resource, APIGROUP column is config for apiVersion
- apiVersion
    - $ kubectl api-versions # list api-versions
- metadata
    - only name is required
- spec
    - all action
    - $ kubectl explain services --recursive # list all resource, key-valuetype
    - $ kubectl explain services.spec
    - $ kubectl explain deployment.spec.template.spec.volumes.nfs.server # explain
---
- dry-run
    - update configmap, secret
    