#Track001 - github

---
1. git vs github
- git - 로컬에 파일의 변경이력 ( 내 컴퓨터의 타임머신)
- gitbut - 클라우드올려서 협업(친구들과 공유작업공간)

---
2. 기본명령어
`git init` 저장소 생성 (빈상자 만들기 )
`git add.` 변경된 파일 추가 (상자에 그림넣기)
`git commit -m "설명" ` 저장 (그림에 이름붙여저장)

---
3. [실습1] github 회원가입 및 로그인
-  https;//github.com/

---
4. [실습2] github 저장소
- 오른쪽 상단 - [+] - [New Repository]

---
5. [실습3] git
- git-scm.com
- 다운로드 - [설치] 
   - ■(New!) Add a Git Bash Profile to Windows Termial

---
6.[실습4] git
6-1.  Gitbash 이름, 이메일 설정정보

6-2. git init   로컬상자만들기

6-3. git add. 파일만들고 상자에 파일 넣기

6-4. git status 상태확인

6-5. git commit -m "first commit" 뭘저장했는지 이름붙이고 저장

6-6. git remote add origin `깃허브주소( 원격저장소 - 공유작업)`

```bash
git remote add origin https://github.com/swc2074/fullstack_20250825.git
```



6-7. git romote -v 연결확인

6-8. git push origin master  원격저장소에 올리기

---
7.[실습5] git 수정후 (ctrl + s) 다시 올리기

``` bash
파일 수정
git add .
git commit -m "git 수정후 다시올리기"
git push origin master
```

---
8. 트러블슈팅

8-1. 문제 코드
``` bash
TJ-BU-703-P03@DESKTOP-5CVIKGS MINGW64 /c/KIMYOUNGMIN/workspace (master)
$ git commit -m "git 수정 후 다시올리기"
On branch master
Changes not staged for commit:
  (use "git add <file>..." to update what will be committed)
  (use "git restore <file>..." to discard changes in working directory)       
        modified:   day001.md

no changes added to commit (use "git add" and/or "git commit -a")
```

8-2. 해결방안
``` bash
- 아래방법을 했는데도 처리안됨
- 너무나도 단순한 이유였음 ! *** 저장안함***

---

### ✅ 해결 방법

1. **수정된 파일을 스테이지에 추가하기**
   ```bash
   git add day001.md
   ```

2. **다시 커밋하기**
   ```bash
   git commit -m "git 수정 후 다시올리기"
   ```

---

### 💡 참고 옵션

- 만약 여러 파일을 한 번에 추가하고 싶다면:
  ```bash
  git add .
  ```
  또는
  ```bash
  git commit -am "메시지"
  ```
  단, `-am` 옵션은 **이미 Git에 추적되고 있는 파일만** 커밋할 수 있어요. 새로 만든 파일은 반드시 `git add`로 먼저 추가해야 합니다.

---


```

> Q. 현재수정된  파일 올리기
