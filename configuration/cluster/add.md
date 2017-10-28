### 2.3.1 클러스터 추가

클러스터를 추가하여 사용할 수 있습니다.

##### a\) 환경설정 -&gt; 클러스터 -&gt; 오른쪽 상단 + 모양의 버튼을 클릭합니다.![](/image.kh/image.kh/클러스터추가1.png)

##### b\) 프로바이더 선택 및 이름, 설명, 클러스터 옵션을 선택합니다.![](/image.kh/image.kh/클러스터추가2.png)

| **클러스터 옵션** | **설명** |
| :--- | :--- |
| 인그레스 지원 | 인그레스 호스트에 subpath로 서비스 노출하는 방식 |
| 로드밸런서 지원 | 로드밸런스 기능 지원 |
| 퍼시트턴트 볼륨 지원 | Public cloud스토리지 및 외부 스토리지 사용 가능 |
| 노드포트 지원 | 노드에 포트를 붙여 서비스 노출하는 방식 |

* **인그레스 지원**![](/assets/인그레스.png)인그레스 방식에 사용할 host ip 주소로 마스터 노드 ip주소를 입력한다.\(마스터 노드 L4 구성 시 L4 VIP 입력\)

* **노드포트 지원**![](/assets/노드포트.png)노드 포트 방식에 사용할 ip 주소로 마스터 노드 ip주소를 입력한다.\(마스터 노드 L4 구성 시 L4 VIP 입력\)

* **클러스터 유형**

  * 기본값으로 cube 선택![](/assets/큐브클러스터정보.png)
    | k8s 버전 | 1.6.7 \(칵테일에서 사용중인 쿠버네티스 버전\) |
    | :--- | :--- |
    | 마스터 URL | 쿠버네티스 마스터 IP \(L4 구성 시엔 L4 VIP\) |
    | 모니터링 호스트 | InfluxDB 설치 IP \(칵테일 모니터링을 위해 InfluxDB사용\) |
    | 모니터링 포트 | 30315 \(influxDB 기본 포트\) |
    | 모니터링 사용자 | root \(influxDB 사용자 ID\) |
    | 모니터링 비밀번호 | root \(influxDB 사용자  Passwd\) |

* 큐브 클러스터 유형

  * MANAGED \(구글 프로바이더 선택시 GKE도 선택 가능\) 선택
  * 인증유형 : certification![](/assets/certification.png)ㄴㅇㄹㄴㅇ
  * ㄴㅇㄹ
  * 
  | 사용자 아이디 | admin |
  | :--- | :--- |
  | 패스워드 | AdminPass |
  | Certificate CA Certification | 마스터 서버 접속 후  /etc/kubernetes/pki 경로 이동 후 ca.pem파일 값  입력 |
  | Certificate Authority Data | 마스터 서버 접속 후 /etc/kubernetes/pki 경로 이동 후 apiserver-key.pem 파일 값 encode 후 입력 |

* 인증유형 : token  
  ![](/assets/token.png)

| Bearer Token | 토큰방식으로 쿠버네티스 인증할 경우 사용 |
| :--- | :--- |


* 프로젝트 ID \( GKE 사용 시에만 필요하며 구글 클러스터를 구성한 프로젝트 아이디를 입력\)![](/assets/프로젝트아이디.png)



