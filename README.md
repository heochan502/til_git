# Git

## 1. Git 프로그램 설치 
 - 프로그램 다운로드 https://git-scm.com/
 - 64-bit Git for Windows Setup.

 ## 2. Git 버전 확인
 - 윈도우 키보드 + R 키보드 : `cmd` 입력 
 ```bash
    git --version
 ```

 - 출력창 확인

## 3. VSCode 에 Git 설정하기

### 3.1 터미널 환경을 git bash로 설정하기
 - 윈도우, 맥, 리눅스 의 명령창을 통일 하기 위함.
 - 관리도구 클릭 > 설정메뉴 선택 
 - 설정화면 > `default:Windows` 입력 
 - `Git Bash` 선택
 - 설정화면 닫고, VSCode 재실행 추천

### 3.2. VSCode 에서 Git 옵션 설정하기 
 - 터미널 실행 : ` Crtl + 백틱 ` 추천
 - git 버전확인

```bash
    git --version
```
 
 - 기본 브렌치명을 `main` 으로 설정
 ```bash
    git config --global init.defaultBranch main
 ```
- 윈도우, 맥, 리눅스 환경에서 Enter 키 처리를 통일함.
```bash
    git config --global core.autocrlf true
```
- git commit 명령을 VSCode 에서 작성하도록 설정 

```bash
    git config --global core.editor "code --wait"
```

 - 깃 아이디 설정 하기

 ```bash
    git config --global user.name "아이디"
 ```

  - 깃 아이디 확인 하기

```bash
    git config --global user.name
```

 - 깃 사용자 이메일 저장하기 
 ```bash
    git config --global user.email "이메일"
 ```

 - 깃 사용자 이메일 확인하기

 ```bash
    git config --global user.email
 ```

## 4. 깃작업하기(실습)

### 4.1  깃 프로젝트 관리 초기화 하기

 - 
 ```bash
    git init 
 ```

### 4.2. git 현재 상태 파악 하기

```bash
    git status
```

### 4.3. git 현재 수정된 내용, 파일, 폴더 등을 저장하기 
 
 - 원하는 파일만 저장 하기
```bash
    git add README.md
```

 - 모든 파일 및 폴더 저장하기(추천)
```bash
git add .
```

### 4.4. 수정 내역 메모 남기기

- 한줄 작업 메모

```bash
git commit -m "git 작업 관련 설명글작성"
```

- 여러줄 메모 작성하기(제목, 상세내용)
```bash
git commit
```


# GitHub