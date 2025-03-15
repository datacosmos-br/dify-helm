# Dify Helm Chart
[![Github All Releases](https://img.shields.io/github/downloads/borispolonsky/dify-helm/total.svg)]()

Deploy [langgenius/dify](https://github.com/langgenius/dify), an LLM based chat bot app on kubernetes with helm chart.

## Installation

```bash
helm repo add dify https://borispolonsky.github.io/dify-helm
helm repo update
helm install my-release dify/dify
```

## Supported Components

### Components that could be deployed on Kubernetes in the current version

- [x] core (`api`, `worker`, `sandbox`)
- [x] ssrf_proxy
- [x] proxy (via built-in `nginx` or `ingress`)
- [x] redis
- [x] postgresql
- [x] persistent storage
- [x] extra manifests
- [ ] object storage
- [x] weaviate
- [ ] qdrant
- [ ] milvus

### External components that can be used by this app with proper configuration

- [x] Redis
- [x] PostgreSQL
- Object Storage:
  - [x] Amazon S3
  - [x] Microsoft Azure Blob Storage
  - [x] Alibaba Cloud OSS
  - [x] Google Cloud Storage
  - [x] Tencent Cloud COS
  - [x] Huawei Cloud OBS
- External Vector DB:
  - [x] Weaviate
  - [x] Qdrant
  - [x] Milvus
  - [x] PGVector
  - [x] Tencent Vector DB
  - [x] MyScaleDB

## Contributors

[![Contributors](https://contrib.rocks/image?repo=maskshell/dify-helm)](https://github.com/maskshell/dify-helm/graphs/contributors)
