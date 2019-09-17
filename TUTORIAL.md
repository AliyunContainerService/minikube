# 教程
请根据阿里巴巴易立工程师的[教程](https://yq.aliyun.com/articles/221687)操作，直到minikube start部分。

如果你需要gcr.io的镜像资源，那么你就来对了地方了。首先，阿里云的minikube不提供gcr.io的镜像。你需要一个http的代理。

运行：

```bash
minikube start --docker-env HTTP_PROXY=http://ip:port --docker-env HTTPS_PROXY=http://port:ip --docker-env no_proxy=localhost,127.0.0.1,10.96.0.0/12,192.168.99.0/24,192.168.39.0/24
```

我们可以继续[hello-minikube](https://kubernetes.io/docs/tutorials/hello-minikube/)的教程了。
