+++
title = "Linux 사용법"
date = "2023-05-20T21:29:20+02:00"
tags = ["programming"]
categories = ["programming"]
banner = "img/banners/Linux1.jpeg"
authors = ["Baebyeolha"]
+++
## Linux Shell
#### OS shell
 운영 체제 상에서 다양한 운영 체제 기능과 서비스를 구현하는 인터페이스를 제공하는 프로그램

 CLI(명령줄 인터페이스), GUI(그래픽 사용자 인터페이스)

 
 #### Unix 계열 CLI
     1. 본 셸: sh  2. 배시:bash 3. z셸: zsh (CLI,GUI)

#### Windows CLI
     1. 도스 프롬프트: command.com(과거 윈도우)  2. 명령 프롬프트: cmd.exe  3. 파워쉘: powersell.exe

#### Linux용 GUI
리눅스는 GUI는 독립적으로 설치하여 사용  :  GNOME, KDE

## Linux 사용자와 권한

#### Linux 사용자 계정
리눅스 사용자는 계정을 가지고 로그인을 해서 사용, 비밀번호로 인증

모든 계정은 숫자로 된 UID 값을 가짐, root user: 모든 권한을 가짐(슈퍼튜저),UID 0번  

루트유저가 아닌 사용자 계정 -> 일반 유저

사용자 계정은 /etc/password 파일에서 관리, 사용자 계정 로그인 허용 or 금지 가능

#### Linux 권한 관리
     1. 소유자, 소유자 그룹, 다른 소유자에 대한 권한 설정   2. 읽기/쓰기/실행 권한 설정
#### 루트 권한의 사용
보안 문제로 root 사용자 계정을 사용할 수 없게 설정하는 경우가 많음 이때 sudo 명령어로 일반 사용자 계정이 root 권한으로 명령을 실행할 수 있음

/etc/sudoers 파일에서 sudo 명령을 사용할 수 있는 사용자 계정 지정

## Linux 기본 명령

#### 셸
     1. 셸 확인:ps   2. 셸 변경: 셸 프로그램 실행(sh,bash,zsh 설치)  3. 셸 탈출:exit

#### 디렉토리
      디렉토리 위치: 절대경로(루트 디렉토리부터), 상대 경로(현재 디렉토리부터)
      /: 루트 디렉토리
      ~: 홈 디렉토리
      ..: 상위 디렉토리
      .: 현재 디렉토리
      이동은 cd로 단, 읽기 권한이 없으면 이동 불가

#### 파일 
      1. 파일속성: chown (소유자 수정), chmod(권한 수정)
      2. 파일 다루기
         mkdir 디렉토리 만들기
         rmdir 디렉토리 지우기(빈 디렉토리만 가능)  // rm: 빈 파일 아니더라도 가능(강력 옵션 rm -rf)
         cp: 복사(하위 디렉토리까지)
         touch: 빈 파일 만들기 
         mv: 파일이나 디렉토리 옮기거나 이름 변경
         find: 파일 찾기

#### 텍스트 파일 보기
     파일 보는 명령어
     more
     cat
     head[-n 줄수] : 맨 앞의 10줄만 (n에서 설정한 줄 수만큼)
     tail[-n 줄수]: 맨 뒤의 10줄만 (n에서 설정한 줄 수만큼)
     grep: 지정된 문자열이 포함된 행만




