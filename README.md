# k8-helm
* installing helm
```
# for ARM systems, set ARCH to: `arm64`, `armv6` or `armv7`
ARCH=x86_64
PLATFORM=$(uname -s)_$ARCH

curl -LO "https://github.com/weaveworks/eksctl/releases/latest/download/eksctl_$PLATFORM.tar.gz"

tar -xzf eksctl_$PLATFORM.tar.gz -C /tmp && rm eksctl_$PLATFORM.tar.gz

sudo mv /tmp/eksctl /usr/local/bin
```