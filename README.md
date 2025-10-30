# Newflix / Shinsegaeflix (web\_making\_basic\_practice00)

OTT 서비스 '신세계플릭스'의 랜딩/로그인 및 컨텐츠 검색 페이지를 구현한 정적(static) 웹사이트 프로젝트입니다. HTML과 CSS의 기본 구조, 특히 모듈형 CSS(@import, 변수) 사용법을 연습하는 것을 목표로 합니다.

단순한 구조로 HTML을 활용하여 정적 웹 페이지를 만들고, 웹 페이지를 이동하는 프로세스를 이해하는 것이 주요 과제입니다.

## 🚀 Live Demo

이 프로젝트는 `.github/workflows/static.yml` 파일에 GitHub Actions 워크플로우가 설정되어 있습니다. `main` 브랜치에 푸시(push)될 때마다 GitHub Pages로 자동 배포됩니다.

배포가 완료되면 `https://[GitHub_Username].github.io/[Repository_Name]/` 주소에서 확인할 수 있습니다.

## ✨ 주요 기능

  * **로그인 페이지 (`index.html`)**
      * 'Shinsegaeflix'라는 서비스명과 함께 아이디/비밀번호 입력 폼을 제공합니다.
      * '접속하기' 버튼을 누르면 'find.html' 페이지로 이동합니다.
  * **컨텐츠 검색 페이지 (`find.html`)**
      * '검색하기' 기능을 위한 검색창이 있습니다.
      * 메인 추천 영화('승리호')를 보여주는 배너가 있습니다.
  * **마이 페이지 (`mypage.html`)**
      * 현재 기본 HTML 페이지만 생성되어 있습니다. (향후 프로필, 이어보기, 찜한 목록 등을 위한 이미지 리소스가 `image/` 폴더 내에 포함되어 있습니다.)

## 📂 프로젝트 구조

```
web_making_basic_practice00/
├── .github/
│   └── workflows/
│       └── static.yml       # GitHub Pages 자동 배포 워크플로우
├── css/
│   ├── global.css         # 전역 스타일 (폰트, 배경색, 공용 클래스)
│   ├── reset.css          # 브라우저 기본 스타일 초기화
│   ├── variable.css       # CSS 변수 (색상 테마) 정의
│   ├── login.css          # 로그인 페이지 전용 스타일
│   ├── find.css           # 검색 페이지 전용 스타일
│   └── mypage.css         # 마이 페이지 전용 스타일
├── image/
│   ├── login-img.png
│   ├── find-bestMovie-img.jpg
│   └── ... (기타 페이지에 사용되는 이미지 리소스)
├── index.html             # 로그인 페이지
├── find.html              # 컨텐츠 검색/발견 페이지
└── mypage.html            # 마이 페이지 (구현 중)
```

## 🛠️ 기술 스택 및 특징

  * **HTML5**
  * **CSS3**
      * **CSS 변수 (Custom Properties)**: `variable.css`에서 `--purple`, `--background-purple` 등 색상 테마를 중앙에서 관리합니다.
      * **`@import`**: `global.css`를 중심으로 `reset.css`, `variable.css` 등 스타일시트를 모듈식으로 불러옵니다.
      * **Flexbox**: `.display-flex-center` 등 페이지 레이아웃에 적극적으로 활용됩니다.
      * **미디어 쿼리**: `login.css` 및 `find.css`에 포함된 간단한 반응형 웹 디자인을 적용했습니다.
      * **Google Fonts** 및 **Material Symbols** 아이콘을 사용합니다.

## 💻 실행 방법

1.  이 레포지토리를 로컬 컴퓨터에 클론(clone)합니다.
2.  `index.html` 파일을 웹 브라우저로 열어 실행합니다.
