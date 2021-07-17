## Git 

(**버전**을 통해) 코드 관리 도구



## SCM & VCS

- SCM: Source Code Management (소스 코드 관리)
- VCS: Version Control System (버전 관리 시스템)



## Git?

- 버전 관리 도구
  - 변경 이력 트레킹
  - 언제든 특정 시점으로 이동 가능
- 백업 도구
- 협업 도구



## Git 버전 관리

> 중요: Git은 **폴더 단위**로 코드 관리

- 커밋 == 버전 생성 == 스냅샷 촬영 == 현재 상태 저장



## Git 사용 명령어

1. `git init`

> 특정 폴더를 git으로 관리 시작

* 프롬프트에 **(master)** 표기.

* .git 폴더 생성

  * .git 폴더 삭제시 git 관리 중지

    

2. `git status`

> git에게 상태 확인

- `git init` 직후 `git status` 실행시 아래 화면 표기.

```
On branch master: master라고 하는 branch에 있음.

No commits yet: 아직 commit 한것 없음.

nothing to commit (create/copy/ files and use "git add" to track): commit 할게 없음. (트래킹 하고 싶다면 "git add"사용)
```

- `a.txt` 파일 생성 직후 `git status` 실행시 아래 화면 표기.

```
untracked files: 추적되지 않은 파일이 있음.
  (use "git add <file>..." to include in what will be committed)
        a.txt(빨강)
   commit 될 수 있게 하고 싶으면, "git add <file>"을 사용.

nothing added to commit but untracked files present (use "git add" to track)
```

- `git add a.txt` 직후

```
Changes to be committed: commit 될 사항이 있음.
  (use "git rm -- cached <file>..." to unstage)
        new file:    a.txt (초록)
```



3. `git add [파일명]`

> Staging Area(스냅샷 무대)에 파일 추가



4. `git commit -m "커밋 메시지"`

> **버전을 생성**

- 커밋(버전) 구성 요소
  - 해시(hash)
  - 작성자
  - 날짜
  - 커밋메시지: 버전에 대한 설명

```
[master (root-commit) c244c22] First commit
 1 file changed, 0 insertions(+), 0 deletions(-)
 create mode 100644 a.txt
```



5. `git log`

> 버전(커밋)들의 히스토리(로그)



6. `git config`

> git 설정

- `git config [설정할 내용] [설정할 값]`

  - `git config user.name "Cloud9KTH"`
  - `git config user.email "kth.ryan.steve@gmail.com"`
  - `git config --global`: 전역설정

  ```
  Author identity unknown: 작자 미상
  
  *** Please tell me who you are.
  
  Run
  
    git config --global user.email "you@example.com"
    git config --global user.name "Your name"
    
  to set your account's default identity.
  Omit --global to set the identity only in this repository.
  ```

  