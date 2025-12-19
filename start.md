# endlessx/mintlify 4.0.705

# Getting started

## install image
```bash
docker build -t endlessx/mintlify:4.0.705 . -f Dockerfile
```
## push image to registry
```bash
docker login --username=18616995258@163.com registry.cn-hangzhou.aliyuncs.com
docker tag [ImageId] registry.cn-hangzhou.aliyuncs.com/endlessx/mintlify:4.0.705
docker push registry.cn-hangzhou.aliyuncs.com/endlessx/mintlify:4.0.705
```
## pull image from Registry
```bash
docker pull registry.cn-hangzhou.aliyuncs.com/endlessx/mintlify:4.0.705
```

## Quickstart
Start mintlify using:
```bash
docker run --name=mintlify -it -d --restart=always  \
  -p 3333:3333 \
  -v /data/mintlify:/var/mintlify \
  -v /etc/localtime:/etc/localtime:ro \
  registry.cn-hangzhou.aliyuncs.com/endlessx/mintlify:4.0.705
```