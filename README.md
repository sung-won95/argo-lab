# argo-lab

Argo CD / Argo Workflows 실습 환경.

## 구성
- `cluster/kind-config.yaml` — kind 3노드 클러스터 정의 (control-plane 1 + worker 2)
- `manifests/` — 배포 대상 앱 (Kustomize base + dev/prod overlay)
- `argocd-apps/` — Argo CD Application 정의

## 클러스터 생성 / 삭제
```bash
kind create cluster --config cluster/kind-config.yaml
kind delete cluster --name argo-lab
```
