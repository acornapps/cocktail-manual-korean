### 2.5.1 스토리지 추가

볼륨을 추가하여 사용할 수 있습니다.

##### a\)    환경설정 -&gt; 스토리지  -&gt; 오른쪽 상단 + 모양의 버튼을 클릭합니다.![](/assets/볼륨 추가1.png)

##### b\)    클러스터, 이름, 설명, 정책을 차례로 기입합니다.![](/assets/볼륨 추가4.png)

| **정책** | **설명** |
| :--- | :--- |
| Retain | PersistentVolumeClaim\(PVC\)가 삭제되도 PersistentVolume\(PV\)안에 데이터가 남아있으며, 추후 재사용 할 수 있습니다 |
| Delete | PVC가 삭제되면서 해당 PV도 함께 삭제되고 그안의 데이터도 모두 삭제됩니다. |

##### 

##### c\) 사용하는 스토리지 플러그인에 따라 스토리지 클래스와 파라미터 설정을 해줍니다.

* ##### NFS Dynamic 스토리지 플러그인 사용 시

![](/assets/볼륨 추가2.png)

| 스토리지 플러그인 | Network Dynamic |
| :--- | :--- |
| 정책 | Dynamic 플러그인은 Retain과 Delete 정책을 지원합니다. |
| 스토리지 클래스 이름 | cocktail-nfs\(기본값\) |

* **NFS Static 스토리지 플러그인 사용 시**

NFS static 볼륨은 Retain정책만을 지원하고, 파라미터에 해당 Server와 Path를 추가해야 합니다.

![](/assets/볼륨 추가3.png)

| 스토리지 플러그인 | Network Static |
| :--- | :--- |
| 정책 | Static 플러그인은 Retain 단일 정책을 지원합니다. |
| 스토리지 클래스 이름 | \(비활성화\) |
| 파라미터 | Server : 스토리지의 IP Address                                                   PPath :  mount 경로 |

* **아마존 스토리지 플러그인 사용 시**![](/assets/aws.png)

| 스토리지 플러그인 | AWS EBS \(AWS의 스토리지 서비스\) |
| :--- | :--- |
| 스토리지 클래스 이름 | **default\(고정값\)** |
| 파라미터 | **파라미터 값 없음** |

* **구글 스토리지 플러그인 사용 시**![](/assets/구글.png)

| 스토리지 플러그인 | Google Persistent Disk \(GCP의 스토리지 서비스\) |
| :--- | :--- |
| 스토리지 클래스 이름 | **standard\(기본값\)** |
| 파라미터 | **type : **구글 스토리지 클래스의 유형 값**                                      zone : **스토리지 생성된 zone 값 |

* **Azure 스토리지 플러그인 사용 시**![](/assets/azure.png)

| 스토리지 플러그인 | Azure Disk \(Azure의 스토리지 서비스\) |
| :--- | :--- |
| 스토리지 클래스 이름 | **default\(기본값\)** |
| 파라미터 | **파라미터 값 없음** |



