# disconf指南

## 依赖

> 项目依赖的镜像来自于 https://github.com/caiwenhao/image.git
> 项目源码 https://github.com/caiwenhao/disconf.git
> mysql zk redis 均使用k8s官方repo

```shell
#添加官方repo
helm repo add stable https://kubernetes-charts.storage.googleapis.com/ 
helm repo add incubator https://kubernetes-charts-incubator.storage.googleapis.com/
```

## 涉及的helm操作

```shell
#需要进入项目目录
cd disconf
#获取依赖包
helm dependency update
#验证语法
helm lint .
#本地安装
helm install . --namespace=disconf --name=disconf
#本地升级
helm  upgrade  disconf .
```

## 知识点

1.多容器pod通过共享卷实现文件共享
2.configmap的变量应用

## 部署
```

```