HowtoUseGitHub
===
- repository는 깃허브 내에서 "나만의 공간" 같은 것

- Public은 해당 repository 안의 모든 자료를 모든 유저가 열람 가능, 업로드는 제한 가능
- Private은 열람과 업로드 모두 제한 가능

Root Folder 연결법
---
1. 원하는 위치에 폴더를 생성한다
2. 폴더 오른쪽 클릭 후 *Git Bash Here* 클릭
3. *git init*
4. *git remote add origin [repository address]*

Push 전엔 Pull이 있다
---
- *git pull origin master* - 지정해놓은 repository에서 해당 폴더로 repository에 있는 모든 자료를 끌어옴
- *git status* - 현재 나의 로컬 폴더와 git 사이의 sync 확인
- *git add .* - 로컬 폴더와 git repository 사이에 변경점이 있을 때, 모든 변경점을 tracking
- *git commit -m "[message]"* - 어떤 변경 사항을 업로드 했을 때, message를 포함해서 실행
- *git push origin master* - git의 push를 요청


내 로컬 폴더에서 실습
---
1. 로컬 폴더 내에 txt 파일 생성
2. 로컬 폴더 오른쪽 클릭 후 *Git Bash Here* 클릭
- 아직 아무것도 push하지 않은 상태이기 때문에 pull하지 않고 진행
3. *git status*
4. *git add .*
5. *git commit -m "Hello GitHub"*
6. *git push origin master*

타인의 Git 가져오기 실습
---
1. 폴더 생성 후 *git init*
2. *git remote add origin [repository address]*
3. *git pull origin master*

- 파일 수정 후 위와 동일한 과정을 거쳐 push를 한다면, 파일의 *History*에서 변경 사항 등을 확인 가능
- GitHub에서 수정 후 *git pull origin master* 하면 로컬 폴더에 변경 사항 적용
