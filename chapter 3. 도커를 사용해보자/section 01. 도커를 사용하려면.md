## 도커를 사용하려면

### 도커는 기본적으로 리눅스용이지만 윈도우와 macOS에서도 사용할 수 있다.
도커엔진이라는 무료 소프트웨어를 설치해야한다.

#### 도커 환경을 구축하는 세가지 방법
- 리눅스 컴퓨터에서 도커 사용하기
- 가상 머신이나 렌탈 환경에 도커를 설치하고 윈도우나 macOS를 통해 사용하기
- **윈도우용/macOS용 도커 사용하기 (채택)**

### 윈도우용/macOS용 도커 사용하기

도커 데스크톱 : 리눅스 운영체제가 들어있는 패키지 (리눅스 운영체제 등의 실행환경이 추가로 필요하기 때문에 패키지로 묶어 함께 배포한다)
![도커 데스크톱](https://github.com/user-attachments/assets/ad3b77cd-cb28-4386-b175-81d33462f105)

#### 도커 데스크톱은 일반적인 소프트웨어처럼 사용한다
- 가상화 소프트웨어나 리눅스 os의 존재를 신경쓰지 않아도 된다

### 도커를 실행하기 위한 조건
- 64비트 운영체제!

#### mac os 버전의 사용조건
- 2010년 이후에 발매된 모델
- macOS 10.13(하이 시에라) 이후 버전
- 메모리 : 4GB 이상

### 도커 데스크톱 설치

공식 사이트에서 다운로드 
- https://docs.docker.com/desktop/install/mac-install/

성공적으로 설치된 도커 데스크톱 화면
<img width="1268" alt="image" src="https://github.com/user-attachments/assets/63b1603f-9298-4360-9784-04844c8b04d8">

----
도커 상태 확인
- docker info
실행 중인 컨테이너 확인
- docker ps
