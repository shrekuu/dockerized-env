# 本地与服务器 Docker 配置

> Mac 与 Linux 系统下, 用 Docker 起多个 php-fpm

## 安装 Docker, 使用阿里镜像

```sh
curl -fsSL https://get.docker.com | bash -s docker --mirror Aliyun
```

## 安装 Compose(仅 Linux)

```sh
sudo curl -L "https://github.com/docker/compose/releases/download/1.27.4/docker-compose-$(uname -s)-$(uname -m)" -o /usr/local/bin/docker-compose
```

