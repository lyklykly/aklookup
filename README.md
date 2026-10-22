# 정답 사전 · Answer Finder

다섯 권의 학습지/워크북 정답지를 전자사전처럼 즉시 찾아주는 웹 앱입니다.
서버나 빌드 과정 없이 `index.html` 파일 하나로 동작합니다.

- **정호 리딩** (Daily Reading Comprehension, EMC 3454) — 주차(Week) · 일차(Day)로 조회
- **Vocabulary Workshop Level A** — 유닛(Unit) · 유형(Category) · 문제 번호로 조회
- **Vocabulary Workshop Level Green** — 유닛(Unit) · 유형(Category) · 문제 번호로 조회
- **Nonfiction Reading Practice, Grade 2** (EMC 3313) — 페이지(Page)로 조회
- **Spectrum Math, Grade 2** — 페이지(Page)로 조회 (p19~p143). 세로셈은 가로식으로, 정답지에서 동그라미 친 답은 동그라미로, 그래프·도형 답은 원본 그림으로 표시

모든 정답 데이터는 제공된 원본 PDF/엑셀 정답지에서 추출해 파일 안에 내장되어 있으며,
인터넷 연결 없이도 (더블클릭으로) 그대로 열립니다.

## 로컬에서 열어보기

`index.html` 파일을 다운로드해서 브라우저로 더블클릭하면 바로 실행됩니다.

## GitHub Pages로 배포하기 (무료 링크 만들기)

1. 이 저장소를 GitHub에 올린 뒤, 저장소 페이지에서 **Settings → Pages**로 이동합니다.
2. **Build and deployment → Source**를 `Deploy from a branch`로 설정합니다.
3. **Branch**를 `main` (또는 `master`), 폴더는 `/ (root)`로 선택하고 **Save**를 누릅니다.
4. 1~2분 후 `https://<사용자아이디>.github.io/<저장소이름>/` 주소로 접속하면 앱이 바로 열립니다.

> `index.html`이라는 파일명이 중요합니다 — GitHub Pages는 이 이름의 파일을 저장소 루트에서 자동으로 첫 화면으로 인식합니다.

## 폴더 구성

```
.
├── index.html   # 앱 전체 (HTML + CSS + JS + 정답 데이터)
└── README.md
```

## 데이터 출처

- Daily Reading Comprehension (EMC 3454), © Evan-Moor Corp. — 제공된 답지 PDF에서 추출 후 원본 이미지와 대조 검증
- Vocabulary Workshop Level A / Level Green 정답 엑셀 파일에서 추출
- Nonfiction Reading Practice, Grade 2 (EMC 3313), © Evan-Moor Corp. — 제공된 답지 PDF에서 추출 후 원본 이미지와 대조 검증
- Spectrum Math, Grade 2 — 제공된 답지 PDF에서 추출 후 PDF 텍스트와 숫자 단위로 대조 검증

개인 학습 용도로 제작된 도구이며, 원본 교재의 저작권은 각 발행사에 있습니다.
