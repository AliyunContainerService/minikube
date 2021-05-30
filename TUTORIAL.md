# 教程
请根据阿里巴巴易立工程师的[教程](https://yq.aliyun.com/articles/221687)操作，直到minikube start部分。

根据这个[教程](https://yq.aliyun.com/articles/29941)申请一个阿里云镜像加速地址。比如说是https://t1ch2dci.mirror.aliyuncs.com
运行：

```bash
minikube start --docker-env HTTP_PROXY= --docker-env HTTPS_PROXY= --image-mirror-country='cn' --image-repository='registry.cn-hangzhou.aliyuncs.com/google_containers' --iso-url='https://kubernetes.oss-cn-hangzhou.aliyuncs.com/minikube/iso/minikube-v1.3.0.iso' --registry-mirror=ttps://t1ch2dci.mirror.aliyuncs.com
```

我们可以继续[hello-minikube](https://kubernetes.io/docs/tutorials/hello-minikube/)的教程了。
