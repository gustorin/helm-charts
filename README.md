# Helm Chart Repository

## Overview

이 저장소는 [Helm](https://helm.sh/)을 사용하여 Kubernetes 애플리케이션을 관리하기 위한 차트 모음을 제공합니다. 각 차트는 특정 애플리케이션 또는 서비스를 배포하는 데 필요한 Kubernetes 리소스를 포함합니다.

## Contents

- [차트 목록](#차트-목록)
- [설치 방법](#설치-방법)

## 차트 목록

| 구분 | 차트 이름         | 설명                       | 버전    |
|------------------|--------------------------|--------|
| argo | argo-cd          | GitOps를 사용하여 Kubernetes 애플리케이션을 배포하고 관리하기 위한 도구입니다. | 7.7.16  |
| argo | argo-rollouts    | Kubernetes에서 배포 전략을 관리하기 위한 도구로, Canary 배포 및 Blue/Green 배포를 지원합니다. | 2.38.2 |
| argo | argo-workflows   | Kubernetes에서 복잡한 작업을 정의하고 실행할 수 있는 워크플로우 관리 도구입니다. | 0.45.4  |
| argo | argo-events      | 이벤트 기반 아키텍처를 위한 Kubernetes 이벤트 관리 도구입니다. | 2.4.13  |
| auth | keycloakx                    | OAuth2 및 OpenID Connect 기반의 인증 및 권한 부여를 제공하는 Identity 및 Access Management 솔루션입니다. | 2.2.2  |
| cnpg | cnpg-cluster     | PostgreSQL 클러스터를 Kubernetes에서 관리하기 위한 Cloud Native PostgreSQL 솔루션입니다. | 0.2.0  |
| cnpg | cloudnative-pg   | PostgreSQL의 클라우드 네이티브 배포 및 관리 솔루션으로, 고가용성과 스케일링을 지원합니다. | 0.23.0  |
| metrics | victoria-metrics-k8s-stack   | 고성능의 시계열 데이터베이스 및 모니터링 솔루션으로, Kubernetes에 최적화되어 있습니다. | 0.33.5  |
| git  | gitea            | Git 서비스와 협업 기능을 제공하는 경량화된 코드 호스팅 플랫폼입니다.        | 10.6.0 |
| repository | harbor                       | 컨테이너 이미지 및 Helm 차트를 저장하고 관리하기 위한 레지스트리입니다.     | 1.16.2 |
| repository | nexus                       | 다양한 형식의 아티팩트를 저장하고 관리하기 위한 유연한 레지스트리 솔루션입니다.	     | 64.2.0 |
| storage | longhorn                     | Kubernetes에서 블록 스토리지를 제공하는 오픈 소스 분산 스토리지 시스템입니다. | 1.7.2  |
| storage | minio                        | 고성능 객체 스토리지 솔루션으로, S3 API 호환성을 제공합니다.                 | 5.4.0  |

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
