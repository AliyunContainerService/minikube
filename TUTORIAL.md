# 教程
请根据阿里巴巴易立工程师的[教程](https://yq.aliyun.com/articles/221687)操作，直到minikube start部分。

如果你需要gcr.io的镜像资源，那么你就来对了地方了。首先，阿里云的minikube不提供gcr.io的镜像。你需要一个http的代理。

运行：

```bash
minikube start --docker-env HTTP_PROXY= --docker-env HTTPS_PROXY= --image-mirror-country='cn' --image-repository='registry.cn-hangzhou.aliyuncs.com/google_containers' --iso-url='https://kubernetes.oss-cn-hangzhou.aliyuncs.com/minikube/iso/minikube-v1.3.0.iso' --registry-mirror=https://t0pp2aci.mirror.aliyuncs.com
```

我们可以继续[hello-minikube](https://kubernetes.io/docs/tutorials/hello-minikube/)的教程了。
