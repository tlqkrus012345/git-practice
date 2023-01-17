wiki, readme : https://github.com/tlqkrus012345/git-practice/wiki

git config --global user.name (이름) : 최초 전역 이름 설정

git config --global user.name : 이름 확인

git init : 깃이 관리 시작

untracked : git의 관리에 들어간 적 없는 파일

git reset vs git revert : reset은 돌아간 시점을 기준으로 앞의 기록을 지운다. revert는 전 단계에서 수행한 작업을 반대로 커밋을
추가한다. 내역을 유지하고 싶으면 revert를 사용

git revert --no --comit (해시코드) : revert 하고 더 추가할 내용이 있을 때 사용

branch : 프로제특를 하나 이상의 모습으로 관리해야 할 때

git merge vs git rebase : merge는 두 브렌치를 합친다 하나의 커밋으로 rebase는 브랜치의 마디들을 메인 브랜치에 옮긴다.

git merge --abort : 당장 충돌 해결이 어려울 경우

git rebase 충돌시 : 수정 -> git add. -> git rebase --continue

git remote add origin (원격 저장소 주소) : 로컬의 git 저장소에 원격 저장소로의 연결 추가 , 원격 저장소 이름 origin 수정 가능

git push -u origin main 어느 원격 브랜치에 푸시할거냐, 이후에는 git push 만 가능

git remote, git remote -v

push와 pull 동시상황 : git pull --no-rebase (merge방식) git pull --rebase(rebase)방식

git은 3가지 파일 상태로 관리 : working directory(untraked, tracked)에서 add하면 staging area에서 
commit하면 repository

git restore --staged (파일명) : staging area에서 working directory

git restore (파일명) : working directory에서도 제거

reset은 세 가지 옵션 : soft(repository -> staging area), mixed(default)(repository -> working directory),
hard(완전한 삭제)

git checkout HEAD~~ : HEAD 두 단계 뒤로

git checkout - : 앞에 했던 단계로 

fetch : 원격 저장소의 최신 커밋을 로컬로 가져오기만 한다. 
main branch에서 fetch 후 origin/main branch에서 변경사항을 확인 후에 main branch에서 pull을 진행한다.
branch역시 마찬가지로 origin/brabch를 확인하고 main에서 git switch -t origin/branch 실행을 진행한다.
