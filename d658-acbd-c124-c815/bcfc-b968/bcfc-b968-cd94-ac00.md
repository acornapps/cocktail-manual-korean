2.5.1    볼륨 추가

  
a\)    환경설정 -&gt; 서비스 -&gt; 오른쪽 상단 + 모양의 버튼 클릭![](/image.kh/image.kh/볼륨 추가1.png)

b\)    클러스터, 이름, 설명 등 상세정보 기입![](/image.kh/image.kh/볼륨추가2.png)

| 정책 | 설명 |
| :--- | :--- |
| Retain | PersistentVolumeClaim\(PVC\)가 삭제되도 PersistentVolume\(PV\)안에 데이터가 남아있다.데이터 옮긴 후 해당  PV사용 가능하다. |
| Recycle |  |
| Delete | PVC가 삭제되면서 해당 PV도 함꼐 삭제되고 그안의 데이터도 삭제된다. |

| 스토리지 플러그인 | 설명 |
| :--- | :--- |
| Network File System |  |
| AWS EBS | Amazon |
| Google Persistent Disk |  |
| Azure Disk |  |



