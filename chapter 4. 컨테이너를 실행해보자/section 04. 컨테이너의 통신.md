<img width="499" alt="image" src="https://github.com/user-attachments/assets/0411e824-9cdf-419d-a719-54c945cea3d0"><img width="319" alt="image" src="https://github.com/user-attachments/assets/984f9a54-a993-42c3-81ac-6c77e3fe5b0d">## 컨테이너의 통신

### 아파치란

- 웹 서버 기능을 제공하는 소프트웨어
- 아파치가 동작중인 서버에 파일을 올려두면 웹 사이트 형태로 볼 수 있다.

### 컨테이너와 통신을 하려면
포트 설정이 필요하다

- 포트 : 통신 내용이 드나드는 통로를 의미한다

> 포트 설정 방법
>
>  -p 호스트포트번호:컨테이너포트번호

컨테이너를 사용하면 여러개의 웹서버를 함게 실행 할 수 있다.
이런경우 호스트포트번호를 모두 같은 것으로 사용하면 어떤 컨테이너로 가야 할 요청인지 구분할 수 없기 때문에 구분해줘야한다.
❗ 꼭 여러 컨테이너로 연결되는 포트를 같게 설정하고 싶다면 리버스 프락시로 서버 이름을 통해 구별하도록 구성한다.

### 실습 - 통신이 가능한 컨테이너 생성

step 1) 아파치 이미지를 사용해 apa000ex2라는 이름의 컨테이너를 생성 (port 8088:80)
<img width="750" alt="image" src="https://github.com/user-attachments/assets/0bd05a0d-4213-4763-b03f-bceeb51080ac">

step 2) 컨테이너가 실행 중인지 확인
<img width="881" alt="image" src="https://github.com/user-attachments/assets/b35a0b35-13b1-4f19-aca0-673208a4adc6">

step 3) 웹 브라우저를 통해 아파치에 접근할 수 있는지 확인

<img width="319" alt="image" src="https://github.com/user-attachments/assets/fad36cb2-f2a1-41aa-98e0-a628af4cfcfb">

step 4) apa000ex2 컨테이너 종료

<img width="499" alt="image" src="https://github.com/user-attachments/assets/db9f6b04-c00d-4bd2-8341-237183b47a4e">

step 5) apa000ex2 컨테이너 삭제

<img width="575" alt="image" src="https://github.com/user-attachments/assets/d0f81511-08e7-46bd-90d1-74c4eeeb622a">

step 6) 컨테이너가 삭제됐는지 확인

<img width="651" alt="image" src="https://github.com/user-attachments/assets/a182c595-caf9-4237-af73-eddad1ecd387">

