## 6.1 Kubernetes\(k8s\)

#### 1.Cluster

| 용어 | 설명 |
| :--- | :--- |
| Namespace | k8s의 가상  클러스터로 사용자들이 여러팀 또는 프로젝트로 분산되어 작업 할 수 있는 별도의 환경입니다. |
| Nodes | k8s의 클러스터링되어 있는 어플리케이션을 구동하는 물리서버 또는 VM입니다. |
| Persistent Volumes\(PV\) | 외부 저장소입니다. NFS, iSCSI, 클라우드에서 제공하는 스토리지시스템을 지원합니다. |
| Roles | 사용의 따라 권한을 부여할 수 있습니다. |
| Storage Classes | PV를 동적으로 Provisioning할 경우, NFS 서버를 식별하기 위한 식별자입니다. |

#### 2.Workloads

| 용어 | 설명 |
| :--- | :--- |
| Cron Jobs | '특정 시점에서 한 번' 또는 '특정 시점에서 반복'과 같이 시간 기반의 관리 작업입니다. |
| Deployments | Pod 생성을 위한 설정값의 등록 정보입니다. |
| Jobs | 1개 이상의 Pod를 생성하고 지정된 수의 Pod가 성공적으로 종료되도록합니다. |
| Pods | 1개 이상의 컨테이너로 구성되는 k8s에서 deploy를 위한 최소단위입니다. Pod는 어플리케이션 스택에서 서로 다른 docker image를 혼합하여 구성할 수 있습니다. |
| Replica Sets | 지정된 Pod 복제본이 항상 실행\(유지\)되도록 합니다. |
| Replication Controllers | 지정된 수의 Pod 복제본이 실행되고 있는지 체크합니다. |
| Stateful Sets | Pod의 배포 및 확장을 관리하고, Pod의 순서와 특성에 대한 설정을 제공합니다. |

#### 3.Discovery and load balancing

| 용어 | 설명 |
| :--- | :--- |
| Ingresses | 외부접근에 대한 요청을 name-based로 가상 hosting을 제공합니다. |
| Services | 여러 컨테이너를 하나의 논리적인 단위로 그룹화하여, 외부에서 접속할 수 있는 단일 endpoint를 제공합니다. |

#### 4.config and storage

| 용어 | 설명 |
| :--- | :--- |
| Config Maps | 데이터를 저장하여 사용할 수 있게 지원합니다. |
| Persistent Volume Claime\(PVC\) | 사용자가 PV에 대한 요청입니다. Pod는 PVC를 통하여 리소스\(CPU 및 메모리\)를 요청할 수 있고, 저장공간의 사이즈 및 접근 권한\(rw, readOnly ...\)을 요청할 수 있습니다. |
| Secrets | Password 또는 OAuth 토큰 및 ssh key 등의 저장소입니다. |

#### 5.settings

K8s의Global Settings값을조정할수있습니다.

| 옵션 | 설명 |
| :--- | :--- |
| Cluster name | Kubernetes Cluster의 이름값을 조정할 수 있습니다. |
| Items per page | 1페이지에 나타낼 수 있는 Items의 값을 조정할 수 있습니다. |
| Auto-refresh time interval | Log를 자동으로 새로고침하는 시간을 조정할 수 있습니다. |



