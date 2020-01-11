# clv-stack Helm Chart

创履项目后端程序,主要是快速搭建，管理不同环境的后端程序。

## Prerequisites Details

* Kubernetes 1.8+

## Chart Details 

## Installing the Chart

To install the chart with the release name `my-release`:

```bash
$ helm install --name my-release stable/elastic-stack
```

## Deleting the Charts

Delete the Helm deployment as normal

```
$ helm delete my-release
```

Deletion of the StatefulSet doesn't cascade to deleting associated PVCs. To delete them:

```
$ kubectl delete pvc -l release=my-release,component=data
```

## Configuration
