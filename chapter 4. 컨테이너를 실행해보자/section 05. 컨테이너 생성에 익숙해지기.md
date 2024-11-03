## 컨테이너 생성에 익숙해지기

#### 실습 - nginx 컨테이너 실행하기

step 1) 컨테이너 생성 및 실행
<img width="724" alt="image" src="https://github.com/user-attachments/assets/41abe10c-b226-4fdf-b9e7-8c205383390a">

step 2) ps 커맨드를 통해 컨테이너가 실행중인지 확인
<img width="901" alt="image" src="https://github.com/user-attachments/assets/5ab51771-7c82-4f8d-94f9-ad3975ebd68d">

step 3) 웹브라우저를 통해 nginx 접근
<img width="1101" alt="image" src="https://github.com/user-attachments/assets/76042b80-7ab0-4193-933d-f3dee408d6ff">

step 4) 컨테이너 종료
> docker stop [컨테이너 명]

step 5) 컨테이너 제거
> docker rm [컨테이너 명]

step 6) 컨테이너가 제거 됐는지 확인
> docker ps -a

