### 2.3.1 클러스터 추가

클러스터를 추가하여 사용할 수 있습니다.

##### a\) 환경설정 -&gt; 클러스터 -&gt; 오른쪽 상단 + 모양의 버튼을 클릭합니다.![](/assets/클러추가수정.png)

##### b\) 프로바이더 선택 및 이름, 설명을 작성합니다.![](/assets/클러스터추가2.png)c\) 프로바이더 선택에 따라서 클러스 정보를 입력합니다.![](/assets/클러스터추가3.png)

| **클러스터 정보 ** | **설명** |
| :--- | :--- |
| 리전 | kubernetes 클러스터 서버의 리전.\(물리서버는 Default.\) |
| 인증 유형 | kubernetes 인증 유형.\(Token/Certification\) |
| Ingress Host | 인그레스 방식에 사용할 Host IP Address.\(Master IP or Loadbelancer IP\) |
| 노드 포트 URL | 노드에 포트를 붙여 서비스 노출하는 방식에서 포트 앞에 사용할  IP.\(Master IP or Loadbelancer IP\) |
| 노드 포트 범위 | 노드에 포트를 붙여 서비스 노출하는 방식에서 IP뒤에 사용할 포트의 범위\(30000~32767 권장.\) |
| k8s 버전 | kubernetes 버전에 대한 설명. |
| 마스터 URL | kubernetes API 주소. [https://마스터](https://마스터) IP:6443 형식을 따른다. |
| 모니터링 호스트 | InfluxDB가 설치되어 있는 서버의 IP 주소. |
| 모니터링 포트 | InfluxDB의 포트 정보 |
| 모니터링 사용자 | InfluxDB 사용자 ID\(기본값-root\) |
| 모니터링 비밀번호 | InfluxDB 사용자 PW\(기본값-root\) |

* **인증 유형 - token**![](/assets/클러스터추가token.png)

| 목록 | 설명 |
| :--- | :--- |
| Bearer Token | k8s 설치시 발급한 토큰값 입력. |

* **인증 유형 - certification**![](/assets/클러스터추가certification.png)

| **목록** | **설명** |
| :--- | :--- |
| Cluster CA Certification | 마스터 서버 접속 후 /etc/kubernetes/pki 경로 이동 후 ca.pem파일 값 입력 |
| Client Certificate Data | 마스터 서버 접속 후 /etc/kubernetes/pki 경로 이동 후 apiserver.crt 파일 값 입력 |
| Client Key Data | 마스터 서버 접속 후 /etc/kubernetes/pki 경로 이동 후 apiserver.key 파일 값 입력 |

* **프로젝트 ID \( GKE 사용 시에만 필요하며 구글 클러스터를 구성한 프로젝트 아이디를 입력\)**![](/assets/프로젝트아이디.png)



