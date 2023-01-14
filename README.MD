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