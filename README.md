git config --global core.autocrlf true //윈도우와 맥의 엔터로 인한 오류차이 방지

git config --global user.name "(본인 이름)"
git config --global user.email "(본인 이메일)"

git config --global init.defaultBranch main //기본 브랜치 이름 master->main 변경

시작
git init //처음 프로젝트 시작지 입력 .git 폴더 생성

git status //현재 상태

------------------------------------------

git add "파일이름" //파일 한개만 올려두기
git add . //전체 파일 올려두기

git commit //add 한 내역 타임캡슐에 담기
git commit -m "message" //메시지와 함께 커밋
git log //커밋 내역

git commit -am "message" //add, commit 한꺼번에

------------------------------------------

git reset --hard "reset할 해쉬" //이전 내역들을 전부 삭제
git revert "해쉬" //이전 내역들을 삭제시키지 않고 해당 시점으로 돌아감
git revert --no-commit (되돌릴  커밋 해시) //커밋하지 않고 revert함

------------------------------------------
git merge add-coach  //기록을 남김
git rebase main

-------------------------------------------
git remote add origin (원격 저장소 주소) 
git branch -M main
git push -u origin main 

git remote
git remote remove (origin 등 원격 이름)

git clone (원격 저장소 주소)

git push
git pull
git push --force //강제 푸쉬

git push -u origin from-local
git branch --all

git fetch //저장소 변경 내용 확인
git switch -t origin/from-remote //브랜치 복사하고 변경
