# Helm Chart Repository

## Overview

이 저장소는 [Helm](https://helm.sh/)을 사용하여 Kubernetes 애플리케이션을 관리하기 위한 차트 모음을 제공합니다. 각 차트는 특정 애플리케이션 또는 서비스를 배포하는 데 필요한 Kubernetes 리소스를 포함합니다.

## Contents

- [차트 목록](#차트-목록)
- [설치 방법](#설치-방법)

## 차트 목록

| 차트 이름         | 설명                       | 버전    |
|------------------|--------------------------|--------|
| argo-cd          | GitOps를 사용하여 Kubernetes 애플리케이션을 배포하고 관리하기 위한 도구입니다. | 7.7.16  |
| argo-rollouts    | Kubernetes에서 배포 전략을 관리하기 위한 도구로, Canary 배포 및 Blue/Green 배포를 지원합니다. | 2.38.2 |
| argo-workflows   | Kubernetes에서 복잡한 작업을 정의하고 실행할 수 있는 워크플로우 관리 도구입니다. | 0.45.4  |
| argo-events      | 이벤트 기반 아키텍처를 위한 Kubernetes 이벤트 관리 도구입니다. | 2.4.13  |
| cnpg-cluster     | PostgreSQL 클러스터를 Kubernetes에서 관리하기 위한 Cloud Native PostgreSQL 솔루션입니다. | 0.2.0  |
| cloudnative-pg   | PostgreSQL의 클라우드 네이티브 배포 및 관리 솔루션으로, 고가용성과 스케일링을 지원합니다. | 0.23.0  |
| gitea            | Git 서비스와 협업 기능을 제공하는 경량화된 코드 호스팅 플랫폼입니다.        | 10.6.0 |

## 설치 방법

Helm 차트를 설치하려면 다음 명령어를 사용하세요:

1. Helm 저장소 추가:

```bash
   helm repo add gustorin https://gustorin.github.io/helm-charts
```

2. Helm 저장소 업데이트:

```bash
   helm repo update
```

3. Helm 차트 설치:

```bash
    helm install argo-cd gustorin/argo-cd
```