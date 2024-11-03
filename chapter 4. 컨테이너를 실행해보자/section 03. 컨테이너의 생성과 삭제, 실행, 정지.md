<img width="1008" alt="image" src="https://github.com/user-attachments/assets/2e450aae-cccb-4fbb-9f7e-3067b63c25e9">## 컨테이너 생성과 삭제, 실행, 정지

### docker run 커맨드와 docker stop, docker rm 커맨드

> 컨테이너 실행 : docker run (docker container run)
도커 컨테이너를 실행하려면 이미지가 필요한데, 필요한 이미지가 없다면 이미지를 내려받는 기능도 겸한다.

- 컨테이너 생성 : docker create (docker container create)
- 컨테이너 실행 : docker start (docker container start)
- 이미지 내려받기 : docker pull (docker image pull)
  이걸들을 한번에 하려면! => docker run!

> 2장 참고) 도커 컨테이너 생애주기 : 쓰고 버리는 방식으로 사용
<img width="635" alt="image" src="https://github.com/user-attachments/assets/71669885-3b75-48b1-bebb-b9af04a8c00a">

❗ 컨테이너를 폐기하려면 먼저 컨테이너를 **정지** 시켜야 한다! 동작중인 컨테이너를 그대로 삭제할는 것은 불가능!!

- 컨테이너 정지 : docker stop (docker container stop)
- 컨테이너 삭제 : docker rm (docker container rm)


#### ❓-d /-i, -t
- -d (백그라운드로 실행) 옵션을 붙이지 않는다면 : 컨테이너가 프로그램의 실행을 마칠때까지 터미널의 제어를 차지하므로 그 다음 명령어를 입력할 수 없다
- -i, -t(키보드로 제어) 옵션을 붙이지 않는다면 : 컨테이너 안의 파일 시스템에 접글 할 수 없다

### docker ps 커맨드

현재 실행중인 컨테이너의 목록을 출력 (docker container ls)
- 컨테이너를 실행하거나 정지시킬때 컨테이너의 상태가 기대했던 대로인지 확인
- 컨테이너의 상세 정보를 확인할 때도 사용

> docker ps -a     // 현재 존재하는 컨테이너의 목록 출력

#### 컨테이너의 목록정보

- 첫번째 행 : 각 항목의 이름이 출력
- 두번째 행 : 실제 컨테이너 정보가 출력 (없을수도 있다)

> 확인 가능한 정보 : 컨테이너 ID, 컨테이너를 만들때 사용한 이미지 이름, 컨테이너의 현재상태, 컨테이너의 이름
<img width="622" alt="image" src="https://github.com/user-attachments/assets/addbe0f3-a4b5-4705-9079-be818b5ffa0a">

### 실습 - 컨테이너를 생성하고, 실행, 상태확인, 종료, 삭제해보자

step 1) 아파치 이미지를 사용해 apa00011ex1 이라는 이름의 컨테이너를 생성하고 실행
<img width="714" alt="image" src="https://github.com/user-attachments/assets/1d698acc-7962-40c9-a397-70235ac2f728">


step 2) 컨테이너가 실행중인지 확인!
<img width="1008" alt="image" src="https://github.com/user-attachments/assets/29139cb4-819a-4a8b-9038-bebc95d77591">

step 3) 컨테이너 종료
<img width="501" alt="image" src="https://github.com/user-attachments/assets/180bee60-c62f-46a5-97bc-0c009763bd1d">

step 4) 컨테이너가 종료 됐는지 확인
<img width="597" alt="image" src="https://github.com/user-attachments/assets/74de89e0-7358-4d70-beec-30b2f48740e7">

step 5) ps 커맨드와 인자를 사용해 컨테이너의 존재 여부 확인
<img width="963" alt="image" src="https://github.com/user-attachments/assets/a5fc0391-a284-4964-b38d-ab82cd788b45">

step 6) 컨테이너 삭제
<img width="581" alt="image" src="https://github.com/user-attachments/assets/a508ed5d-1548-48bf-aebf-c98e45704d24">

step 7) 컨테이너가 삭제됐는지 확인
<img width="583" alt="image" src="https://github.com/user-attachments/assets/f7282153-e6ce-4719-819c-5380f5d16712">





