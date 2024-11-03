## 이미지 삭제

컨테이너를 삭제해도 이미지는 그대로 남아있다. 이미지를 삭제하려면 명시적으로 명령을 사용해야 한다

### 이미지 삭제
- 해당 이미지로 실행한 컨테이너 남아있으면 이미지를 삭제할 수 없기때문에 docker ps -a로 컨테이너 목록을 확인하고 컨테이너를 종료해야한다.

### docker image rm

docker rm : container를 삭제하는 명령어다.

#### 이미지를 삭제하는 커맨드 : docker image rm

여러개의 이미지를 한번에 삭제 할 수 있다.
- docker image rm [이미지 이름], [이미지 이름], [이미지 이름]

### docker image ls 커맨드

이미지를 삭제하려면 이미지의 이름 or ID를 알고 있어야 한다

❗ docker ps -a 와 달리 -a 옵션은 사용할 수 없다. 이미지는 컨테이너와 달리 상태(실행중, 종료)를 가질 수 없기 때문이다.

#### 이미지 목록의 정보
<img width="485" alt="image" src="https://github.com/user-attachments/assets/ae53e088-05b8-4ce7-827b-6a948ea90ecc">

### 실습 - 이미지 삭제하기

step 1) 실행한 컨테이너가 있는지 확인
> docker ps -a

step 2) 이미지 목록 확인
> docker image ls

stpe 3) 이미지 삭제
> docker image rm
<img width="822" alt="image" src="https://github.com/user-attachments/assets/90d6d9ef-71c6-4f32-8967-2df9ea1adad0">

