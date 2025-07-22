# CLI 기본 문법
- 현재 디렉토리(.)
- 현재의 상위 디렉토리 (..)
- touch : 파일 생성
- mkdir : 새 디렉토리 생성
- ls : 현재 작업 중인 디렉토리 내부의 폴더 / 파일 목록을 출력
- cd : 현재 작업 중인 디렉토리를 변경(위치 이동)
- start : 폴더 / 파일을 열기
- rm : 파일 삭제(디렉토리 삭제는 -r 옵션을 추가 사용)
- pwd : 현재 작업 중인(디렉토리)의 절대 경로를 출력

# 경로의 핵심 개념
- 루트 디렉토리(/) : 건물의 '정문', 모든 주소의 시작점
- 홈 디렉토리(~) : 나의 '집', 터미널을 처음 켰을 때 시작하는 나의 기본 공간
- 절대 경로 : 누가 어디서 보든 항상 똑같은 주소
- 상대 경로 : 현재 내 위치를 기준으로 한 주소

# git의 3가지 영역
- Working Directory - Staging Area - Repository
- git add : Working Directory에서 Staging Area로 보내기
- git commit -m "~" : Staging Area에서 Repository로 보내기