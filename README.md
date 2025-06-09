# Git 관련 내용

- Git 은 파일의 버전ㅇ르 관리하는 툴

## Git 설치

- https://git-scm.com/

![Image](https://github.com/user-attachments/assets/f7e46368-8fe7-4ed5-b2f4-063a34047481)
![Image](https://github.com/user-attachments/assets/353d2b02-6678-42e9-8414-523238a09043)
![Image](https://github.com/user-attachments/assets/4d34e225-6522-4afa-b079-ab8b2ebf76d4)

- `아래는 반드시 VSCode 설치하고 진행해야 함. (목록 확인 필요)`
  ![Image](https://github.com/user-attachments/assets/c111e424-2037-40a2-8f80-04e29181e432)
- 나머지는 기본값으로 설치 완료 하기.

## Git 사용자 설정

- VSCode 에서 터미널을 `Git Bash` 로 설정함.
- 터미널 실행 단축키 : `Ctrl + ~`
- 셋팅아이콘 선택 > Setting 메뉴 선택
  ![Image](https://github.com/user-attachments/assets/67bb5500-6afd-46ec-9a3b-348b376ed0b5)
- 검색에 '[Terminal default]`입력 >`Git bash` 목록 선택
  ![Image](https://github.com/user-attachments/assets/81566123-8a17-495c-affd-b3d5536aec49)

## Git 정보 확인 및 셋팅 (터미널에서 진행함)

- Git 버전 확인

```bash
git --version
```

- 기본 브렌치명을 `main` 으로 설정하기 (초기 설치시 master 로 되어있음)

```bash
git config --global init.defaultBranch main
```

- Enter 키를 통일시킴(맥, 윈도우, 리눅스가 Enter키, 줄변경이 달리 처리됨)

```bash
git config --global core.autocrlf true
```

- 깃 수정내역, 즉 commit 시 메세지 상세 남기기(VSCode로 작성하도록 셋팅)

```bash
git config --global core.editor "code --wait"
```

- 사용자 설정(아이디, 이메일 : 구글계정과 깃허브 아이디 추천)

```bash
git config --global user.name "아이디"
git config --global user.email "아이디@gmail.com"
```

# GitHub

- 회원가입(http://github.com) : 구글계정
- 예제) til_git 저장소 생성 (생략)

## GitHub 사용자 계정 보안 설정

- 초기 설정시 다음 내용을 필수로 확인한다.

  - `자격 증명 관리자` > Windows 자격 증명 관리 탭 > Git 관련 제거
    ![Image](https://github.com/user-attachments/assets/c1ec3dbb-88a2-4cba-bf21-bfcbe92b7552)

- GitHub 자격 증명 등록은 git push 진행되면 자동으로 로그인 팝업이 출력됨.

## Git 작업 및 GitHub 연결 작업 진행

### 1. 최초 프로젝트 관리를 Git 으로 설정

```bash
git init
```

### 2. 현재 프로젝트 상태 보기

```bash
git status
```

### 3. git으로 파일 추적하기

```bash
git add README.md
```

### 4. git 으로 모든 파일 추적하기

```bash
git add .
```

### 5. 작업히스토리 남기기

- 간단하게 메모 남기기

```bash
git commit -m "메세지"
```
