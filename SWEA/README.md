# SWEA 하루 한 문제

- 시작일: 2026-10-12
- 언어: Python 3
- 목표: 매일 한 문제를 직접 풀고, 정답 확인 후 코드와 짧은 회고를 기록합니다.

## 폴더 구조

```text
SWEA/
├── D1/ ... D8/             # 난이도별 풀이
├── Unrated/               # 난이도가 없는 문제
├── templates/
│   ├── solution.py        # Python 풀이 템플릿
│   └── notes.md           # 문제별 회고 템플릿
└── LOG.md                 # 날짜별 풀이 기록
```

문제 하나당 `D2/1954_달팽이숫자/`처럼 `문제번호_문제명` 폴더를 만들고 `solution.py`와 `README.md`를 넣습니다. 위 경로는 이름 예시이며, 풀이 완료를 뜻하지 않습니다.

## 처음 준비하기

Git과 Python 3를 설치한 환경에서 실행합니다.

```powershell
git clone https://github.com/hojun0/TIL.git
cd TIL
```

이미 TIL을 내려받았다면 해당 폴더에서 `git pull --ff-only`로 최신 내용을 받습니다.

## 매일 하는 순서

1. SWEA에서 오늘 풀 문제를 선택합니다.
2. 난이도 폴더 아래에 문제 폴더를 만들고 템플릿을 복사합니다.
3. 문제의 입력 형식에 맞게 코드를 작성하고, 샘플과 경계 조건을 확인합니다.
4. SWEA에 제출하여 정답을 확인합니다.
5. 문제별 README에 문제 링크·접근 방법·복잡도·배운 점을 적습니다.
6. [LOG.md](LOG.md)에 오늘의 기록을 한 줄 추가한 뒤 커밋합니다.

문제 폴더를 만드는 PowerShell 예시:

```powershell
New-Item -ItemType Directory -Force SWEA/D2/1954_달팽이숫자
Copy-Item SWEA/templates/solution.py SWEA/D2/1954_달팽이숫자/solution.py
Copy-Item SWEA/templates/notes.md SWEA/D2/1954_달팽이숫자/README.md
```

로컬 실행:

```powershell
python SWEA/D2/1954_달팽이숫자/solution.py
```

직접 입력을 붙여 넣거나 IDE의 입력 파일 기능으로 확인합니다. 문제에서 테스트 케이스 수나 출력 형식이 다르면 템플릿도 수정합니다.

업로드 예시:

```powershell
git add SWEA
git commit -m "solve: SWEA D2 1954 달팽이숫자"
git push origin master
```

## 기록 원칙

- 날짜는 한국 시간 기준으로 적습니다.
- 정답 확인 전에는 완료로 기록하지 않습니다.
- 문제 본문 대신 문제 링크와 직접 작성한 풀이·회고를 남깁니다.
- 입력 파일과 실행 결과 등 로컬 실험 파일은 Git에서 제외합니다.
