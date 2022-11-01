# Docker 发布流程

## 构建 Docker 

### 构建 Docker
```
docker build -t continuumio/miniconda3 -f Dockerfile ./
```

## 发布 Docker

### 登录私有仓库
```
docker login -u [USERNAME] -p [PASSWORD] registry.superlucy.net
```

### 设置 Docker 标签
```
docker tag continuumio/miniconda3:latest registry.superlucy.net/continuumio/miniconda3:latest
```

### 推送 Docker 镜像
```
docker push registry.superlucy.net/continuumio/miniconda3:latest
```

## 使用 Docker

### 拉取 Docker
```
docker pull registry.superlucy.net/continuumio/miniconda3:latest
```
