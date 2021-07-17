## Git 백업

> Source code와 version의 관리.
>
> 백업을 하려면 각각의 컴퓨터가 가능하면 가장 멀리 떨어진 곳의 컴퓨터에 백업.
>
> .git 폴더만 클라우드나 다른 곳에 백업 해두면 됨.



#### 1. 용어 정리

- Remote Repository: 원격 저장소
- Local Repository: 로컬 저장소(개인 컴퓨터 or 사무용 컴퓨터)
- host: 인터넷에 연결된 한대 한대의 컴퓨터

- hosting: 인터넷에 연결되어 원격으로 사용할 수 있는 서버를 임대해주는 서비스
- git hosting: 로컬 저장소에 버전을 업로드할 원격 저장소를 임대해 주는 비즈니스
-  **push**, **pull**, **clone** 개념표

| Local 1 -> Remote | Remote -> Local 1 | Remote -> Local 2 |
| ----------------- | ----------------- | ----------------- |
| push              | pull              | clone             |
| backup            | download (다른 부분만)          | copy              |



#### 2. Git hosting

- github: git hosting 서비스중 가장 유명.
- gitlab: 비공개 저장소 무료 제공.



#### 3. 저장소 생성

- github 가입후, "New repository" 로 새로운 저장소 생성.
- 저장소 생성



#### 4. 원격 저장소(Remote repository)와 연결

1. Git Bash 실행
2. `git remote add origin [저장소의 주소]` 입력
   - github 에서 저장소의 주소를 확인.
3. `git remote` or `git remote -v` 입력
   - 원격 저장소(Remote repository)와 연결 확인.



#### 5. git push(backup)

* `git push origin master` 입력하여 git push(backup) 진행.

  

#### 6. git clone(복제 or copy)
* `git clone [저장소]` 입력 하여 github 서버에 저장된 프로젝트 local 저장소에 저장 가능.



#### 7. git pull(다른 부분만 download)

* `git pull [저장소]` 입력하면 기존에 작업하던 부분에서 달라진 부분만 github 서버에서 받아옮.
