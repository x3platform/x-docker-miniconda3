# Miniconda Docker

## Pull Docker 

```
docker pull x3platform/miniconda3
```

## Build Docker
```bash
# login
docker login -u [USERNAME] -p [PASSWORD]

# build
docker buildx build --push --tag x3platform/miniconda3:latest --platform linux/amd64,linux/arm64 --file ./build/Dockerfile ./build/
```
