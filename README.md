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
7. 자유롭게 수정 후 파일 저장
8. 터미널에 `git status` 업로드 안된 파일 빨강색 색 확인
9. `git add 파일명` 수정한 파일 스테이지에 업로드하기
10. `git commit -m '메세지'` 수정 파일에 대한 기록 메세지 작성
11. `git push origin main`  깃허브 저장소에 업로드
12. HTML 속성은 요소에 관한 정보와 기능을 제공합니다
13. HTML 속성은 요소의 동작,연결,기능을 정의합니다
14. HTML 속성은 웹 페이지를 설계하고 구현하는데 필요한 정보를 제공합니다
15. HTML 속성은 웹 표준을 준수하는 동시에 의미론적마크업구조를 구현하는데 도움을 줍니다
----
# HTML 속성의 종류
* 전역 속성: 모든 HTML 요소에서 공통적으로 사용가능한 속성
* 필수 속성: HTML 요소에 필수적으로 사용되어야 하는  속성
* 선택 속성: HTML 요소에 필수적으로 사용되지 않는 속성
* 이벤트 속성: HTML 요소의 이벤트와 관련된 속성
----
# HTML 속성의 작성 규칙
* DTD를 제외한 모든 요소와 애트리뷰트는 소문자로 작성합니다
* 애트리뷰트 값은 큰따옴표("")로 묶습니다
----
# 메타 태그의 특징
* 사이트의 디자인에는 영향을 미치지 않고,문서의 특성을 담고 있습니다
* 문서가 어떤 내용을 담고 있고, 문서의 키워드는 무엇이며,누가 만들었는지 등을 담고있습니다
* HTML 문서에서 BODY태그 앞쪽에 위치하며,일반적으로 HEAD 태그 사이에 위치하게 됩니다