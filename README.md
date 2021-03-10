# 소개
- 여규철 YEO KYUCHEOL
- Mail : mettlekc@gmail.com
- Github : https://github.com/mettlekc

# 경력
### [Netmarble](http://www.netmarble.com)
14/02/03 ~ 현재
- 기술전략 TFT (14/02/03 ~ 14/07/30)
- 모바일 QA (14/08/01 ~ 15/08/02)
- 플랫폼개발팀 (15/08/03 ~ 현재)
- 백앤드 서버 개발

# 보유기술 (관심분야)
### Programming Language
`Java` `Javascript` `Groovy`

### Framework 
`Spring Framework`

### Server
`Apache` `Nginx` `Tomcat`

### Tools
`Spark` `Google PubSub` `Kafka` `Dataflow(Apache Beam)` `Grafana` `ELK` `Jenkins (Pipeline, Blueocean)` `ArgoCD` `Kustomization`

### Database
`MySQL` `MSSQL`

### NoSQL
`Redis` `Aerospike` `Crateio` `Google Bigtable`

### OS
`Linux (Ubuntu, Centos)`

### Environment
`Kubernetes` `Docker`

# 프로젝트 / 운영 서비스
### Kubernetes 배포 CI/CD 구축
##### 기간
- 2020.07 ~ NOW

##### 개발
Kubernetes Container 환경 도입을 위해 Jenkins BlueOcean을 이용한 배포 Pipeline을 구축하였습니다. 
CI/CD 방식의 지속적 통합 배포 할 수 있도록 빌드/설계/테스트/패키지/배포의 네가지 수행단계로 설계 되었으며, 
Gitlab API를 이용하여 릴리즈 노트 생성 자동화 등의 기능도 추가로 지원합니다.

배포는 Kustomization 방식의 배포 정책을 따르도록 구성되었으며, 
ArgoCD에 배포 되도록 준비하였습니다. 
사내 배포 문화 정착을 위해 브랜치 전략과 가이드를 공유하였습니다.

주요기술 

`#Jenkins Blueocean` `#Kustomize` `#Argocd`

### 프로모션

프로모션은 이벤트 또는 프로모션 기간 동안 안내를 위한 웹뷰 정보를 관리하는 서비스입니다.

#### *프로젝트 : 프로모션 결재/노출 제한 기능 개발*
##### 기간
- 2018.03 ~ 2018.08.06

##### 개발
프로모션에 결재 기능을 연동하기 위해 구매 이력을 확인하여 필터링하는 기능과 
웹뷰의 노출 기간을 처리할 수 있는 기능을 개발하였습니다. 
당시 팀 내 Agile 기반 프로젝트 수행 도입이 활발하여 첫 프로젝트로 선정되어 
기획/개발/디자인이 모두 참여한 스크럼 단위 개발을 수행하였습니다.

#### *프로젝트 : 프로모션 레거시 기능 개선*
##### 기간
- 2021.02 ~ NOW
##### 개발
현재 운영되고 있는 프로젝트의 운영 효율성을 높이기 위해 Spring Webflux를 이용하여 
비동기 처리 방식으로 마이그레이션을 수행하고 있습니다. 

- R2DBC를 이용하여 메타데이터 저장소 연동
- Lettuce Redis Cache를 이용하여 메타데이터 캐시


주요기술 

`#Spring Framework` `#Tomcat 9` `#Apache` `#Redis` `#MSSQL`

### 프로필

게임 내 정보(레벨, 친구, 길드정보 등)를 포럼(카페) 서비스에 제공하는 서비스입니다. 
게임마다 다른 데이터를 표준화하고, 
각 게임사에 API를 제공하여 변경된 데이터를 동기화 할 수 있도록 지원합니다. 
또한, 게임 서버(채널) 통합 등의 업데이트 작업 시 데이터 마이그레이션 지원 운영을 하였습니다.

#### *프로젝트 : 프로필 마이그레이션 툴 개발*
##### 기간
2020.01 ~ 2020.03
##### 개발
게임 월드 통합으로 인해 월드별로 구분된 프로필 데이터 통합과 초기화에 대한 요구 사항이 있었습니다. 
Spring Batch를 이용하여 Chunk 단위 마이그레이션 툴 개발하였고, 
Jenkins Pipeline을 연동하여 업무 효율화하였습니다.

주요기술 

`#Spring Framework` `#Tomcat` `#Aerospike` `#Spring Batch` `#Apache Ignite Cache` `#ELK`

### 세그먼트/태그

##### 세그먼트
파일 또는 스트림으로 저장된 그룹 단위 대상 관리 기능

#### *프로젝트 : 구글 파일 업로드 시스템 연동*
##### 기간
2020.02 ~ 2020.04
##### 개발
사내에 GSuit이 도입되어 있기 때문에 CSV 파일 업로드 방식을 구글 파일 드라이브의 스프레드시트를 이용하여 업무 효율화하였습니다. 
업로드 API 및 스프레드시트 불러오기, 구글 OAuth 인증 기능을 내부 관리 툴에서 모두 적용할 수 있도록 파일 업로드 API를 래핑한 
라이브러리 개발하였고, 사내 관리 툴에 적용될 수 있도록 가이드하였습니다.

주요기술 

`#Aerospike` `#Spring Boot` `#Google File Drive` `#Apache Storm`


### 지표
2020.02 ~ NOW

클라이언트/서버 로그 기반 플랫폼 공통 지표를 관리하고 있습니다.
Spark를 이용해 데이터를 Dimension, Metric을 분리, 가공하고, 사용자 정의 지표의 경우 
Google Bigdata로 데이터를 이관하여 서비스하고 있습니다. 

주요기술 

`#Spring Boot` `#Crate.io` `#Apache Spark` `#Google Bigtable` `#Kafka` `#Grafana`

# 활동

###### AWS, GCP 교육 이수

##### (Internship) SK플래닛 ADF 4기
- 2012/07/02 ~ 2012/08/31
- 모바일 애플리케이션 개발

##### (Internship) Ahnlab APC QA 
- 근무기간 : 2010.06.01 ~ 2010.12.31
- QA






