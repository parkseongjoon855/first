# HTML
## Hyper Text Markup Language
### HTML은 웹문서의 구조를 담당하는 언어이다.
* HTML에서 구조는 `<>`로 묶인 태그로 작성한다.
* `<시작태그></닫기태그>`
* `<빈태그>`
* 시작과 닫기태그는 한쌍의 요소로 불린다.
### HTML 구조태그
* HTML5 버전 선언하는 `<!doctype html>`
* HTML 웹브라우저 구조 처리하는 태그들
1. `<html></html>`
2. `<head></head>`
3. ` <body></body>`
----
# git&github
* 버전관리 프로그램 git
* 버전 파일, 폴더들을 저장하는 저장소 github
## git 용어와 뜻
* 작업 디렉터리: 실제 작업하는 로컬 저장소(윈도우 탐색기 개념)
* 스테이징 : 깃허브에 작업 업로드 전 파일을 대기시키는 대기소
* repository : 대기소(stage)에 파일 대기 후 최종 github 업로드 저장소
## 주의사항
* 당일 작업 시작 기준 gibhub 저장소와 로컬저장소의 파일,폴더 상태가 같아야한다.
* 동일한 저장소를 관리하는 사람일 경우  작업 컴퓨터가 달라도 gitconfig에 등록된 이름,이메일이 동일해야 한다.
 ---
 # 주요 단축기 모음
 * `ctrl +/` 한줄 주석
 *  ` shift+alt+a` 선택한 영역만 주석
 ----
 # 처음 git을 이용한 github 저장소 업로드 시 해야하는 순서
 1. 현재 사용중인 로컬 저장소를 git 저장소 등록`git init`
 2. 위 1번 정상 등록 시 경로에 (master) 표시출력
 3. master main으로 최상위 경로명칭을 변경하기 위해 `git branch -m main` 작성
 4. gibhub 저장소 생성후 저장소 주소 복사
 5. 현재 로컬 저장소 github 저장소 연결 `git remote add origin 주소붙여넣기`
 6.  7. 위 6번 결과 파일이 빨강색으로 출력될 경우 `git add 파일명` 스테이징 올리기
 8. `git status` 위 7번에서 올린 파일이 초록색으로 변경된 걸 확인
 9. `git commit -m'기록메세지'` 스테이징 파일을 저장소에 올리기 위한 기록설정
10. `git push origin main` 깃허브 저장소에 최종 파일, 폴더 업로드
11. 위 10번 처음 진행 시 깃허브 계정 인증 화면나오니 인증 진행 후 저장소 f5
----
## 다른 환경에서 이어서 작업해야 하는 경우
1. 폴더 생성하기 vscode 폴더 연결
2. github 저장소 주소 복사
3. vs code 돌아와서 ctri+j 터미널 실행 후 bash 환경 변경
4. `git clone 저장소주소붙여넣기`
5. 터미널 경로 오른쪽에 `main` 또는 `master` 표시가 있는지 확인
6. 위 5번에서 표시가 없다면 `cd 복제한폴더명`
7. 자유롭게 수정 후