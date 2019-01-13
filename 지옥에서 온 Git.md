# 1. 수업소개

## Version Control System - Backup, Recovery, Collaboration

본질적인 요소 : 코드 관리라는 공통된 요소
혁신적인 요소 : CVS, SVN, GIT의 차이점 

*주의) GIT은 아주 복잡하다.

왜 GIT은 어렵지만 광범위하게 사용될까? 

![image](https://user-images.githubusercontent.com/23207379/51083996-6891cf00-1766-11e9-91d2-fc5de88ecf23.png)


# 2. 설치 및 실습방법

# 3. 저장소 만들기

작업을 시작할때 : clone , init 

디렉토리 생성 -> git init

.git : 버전 관리와 관련해서 생성되는 여러가지 정보가 저장된다.

# 4. git이 관리할 대상으로 파일 등록

f1.txt 생성 -> git status -> git add f1.txt -> git status

git status : 버전 관리 상태 표시 
git add : 관리 되고 있지 않은 파일을 git이 관리하도록 등록 (관리 해야 되는 파일이 무엇인지 명확하게 git에게 알려줌)

# 5. 버전 만들기(commit)

지금 까지 작업한 내용을 버전을 만들어서 저장한다.

git status -> f1.txt가 tracking되고 있는 것을 확인 -> git commit -> git log : 1이라는 commit message를 확인 할 수 있다
-> f1.txt 내용을 2로 변경 -> git status : 수정된 사항을 확인 -> git add f1.txt -> git status -> git commit -> git log

# 6. Stage area

f1.txt와 f2.txt모두를 수정

*왜 add 가 존재하는가?) 
commit 하나는 하나의 작업을 담고있는것이 이상적이다. 하지만 그렇게 하지 못했을 경우 add를 이용해서 commit의 크기를 조절할 수 있다.

add명령어를 실행하게되면 commit 대기 상태(stage area)에 들어간다. 

# 7. 변경사항 확인하기

버전을 만든 것의 효용을 알아보자.

* 차이점을 알 수 있다.

git log -p : commit과 commit 사이에 소스상의 차이를 보여준다.

git log 특정커밋번호 : 특정 커밋번호 이전의 커밋을 보여준다.

git diff 커밋번호1..커밋번호2 : 두 커밋의 차이점을 보여준다.

git diff : 방금까지 작업한(수정된) 내용을 보여준다.

# 8. 과거의 버전으로 돌아가기

* 과거로 돌아갈 수 있다. (항상 조심해서 사용할 것 !!)

1. reset

![image](https://user-images.githubusercontent.com/23207379/51084518-8e22d680-176e-11e9-9205-e0dfd50bbc9d.png)

commit 54f4c2eb3513522491241bfe6d179f62705d7013 를 최신으로 하고 싶을 때

git reset 54f4c2eb3513522491241bfe6d179f62705d7013 --hard

2. revert

# 9. 명령의 빈도와 메뉴얼 보는 방법

밑천을 가지고 모르는 것을 물어볼 수 있는 방법만 안다면 어떤 분야에서도 공부 할 수 있다.

매뉴얼 보는것 커뮤니티에 질문하는것 검색하는것 

# 10. 수련해봅시다.

# 11. 
