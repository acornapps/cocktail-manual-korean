### 2.5.1    볼륨 추가

볼륨을 추가하여 사용할 수 있습니다.

##### a\)    환경설정 -&gt; 서비스 -&gt; 오른쪽 상단 + 모양의 버튼 클릭![](/image.kh/image.kh/볼륨 추가1.png)

##### b\)    클러스터, 이름, 설명 등 상세정보를 차례로 기입합니다.![](/image.kh/image.kh/볼륨추가2.png)

| **정책** | **설명** |
| :--- | :--- |
| Retain | PersistentVolumeClaim\(PVC\)가 삭제되도 PersistentVolume\(PV\)안에 데이터가 남아있으며 데이터 이동 후 PV를 재사용 할 수 있습니다 |
| Recycle | 적절한 volume plugin이 있다면 사용한 PV가 다시 새로운 Claim을받을 수 있도록 만들어 줍니다. |
| Delete | PVC가 삭제되면서 해당 PV도 함께 삭제되고 그안의 데이터도 모두 삭제됩니다. |

| **스토리지 플러그인** | **설명** |
| :--- | :--- |
| Network File System | 네트워크 파일 시스템 |
| AWS EBS | Amazon public cloud의 스토리지 서비스 |
| Google Persistent Disk | Google public cloud의 스토리지 서비스 |
| Azure Disk | Microsoft public cloud의 스토리지 서비스 |



