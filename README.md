# 캡처함 개인정보처리방침 페이지

이 저장소는 캡처함(JG Studio KR) 앱의 **외부 공개용 개인정보처리방침**
정적 웹페이지입니다. 서버, 데이터베이스, JavaScript 없이 `index.html`
하나로 완성된 페이지이며, Google Play 콘솔의 개인정보처리방침 URL
항목이나 앱 스토어 등록에 그대로 사용할 수 있습니다.

- 공개 URL: https://jeongkil0486-del.github.io/captureham-privacy/
- 최초 시행일: 2026년 7월 24일
- 개정 및 시행일: 2026년 8월 24일

## 파일 설명

- `index.html` — 개인정보처리방침 전체 내용을 담은 단일 HTML 파일.
  외부 CSS/JS/폰트/이미지를 전혀 불러오지 않으며, 이 파일 하나만
  열어도 완성된 화면이 표시됩니다.
- `README.md` — 이 문서.

## 브라우저에서 확인하는 방법

1. 파일 탐색기에서 저장소 루트의 `index.html`을 더블클릭해 기본 브라우저로 엽니다.
2. 또는 브라우저 주소창에 파일 경로를 직접 입력해도 됩니다.
   예: `file:///C:/FlutterProjects/captureham-privacy/index.html`
3. 인터넷 연결 없이도 정상적으로 표시되는지 확인해 보세요
   (외부 리소스를 전혀 사용하지 않기 때문에 오프라인에서도 동일하게 보입니다).

## GitHub Pages 배포

이 저장소의 `main` 브랜치 루트가 GitHub Pages로 공개됩니다. 정책을 변경할
때는 `index.html`과 이 문서의 개정일 및 내용을 함께 갱신하고, 검토한 변경을
`main`에 반영한 뒤 공개 URL에서 실제 배포 내용을 확인합니다.

현재 방침에는 AI 정밀 분석의 선택·동의 구조, JG Studio KR Cloud Run과
Google Gemini Developer API Paid Service 처리 경로, 익명 설치 ID와 해시 기반
quota 관리, AdMob Rewarded SSV, Google Play Integrity, 그리고 Captureham 서버의
이미지 비영구 저장 정책이 포함되어 있습니다.

## 시행일 수정 위치

`index.html`의 `<header>` 안, 다음 줄을 찾아 날짜를 바꿉니다.

```html
<span class="effective-date">
  최초 시행일: 2026년 7월 24일 · 개정 및 시행일: 2026년 8월 24일
</span>
```

방침 내용을 실제로 변경했을 때만 이 날짜를 갱신하세요.

## 개발자명과 이메일 수정 위치

`index.html`의 "제14조 문의처" 섹션, `contact-box` 안에 있습니다.

```html
<dt>개발자</dt>
<dd>JG Studio KR</dd>
<dt>이메일</dt>
<dd><a href="mailto:captureham@gmail.com">captureham@gmail.com</a></dd>
```

이메일 주소를 바꿀 경우 `href="mailto:..."`와 화면에 보이는 텍스트
두 곳을 모두 같은 주소로 수정해야 합니다.

## 공개 후 확인해야 할 항목

- [ ] 공개된 URL이 모바일과 PC 양쪽에서 가로 스크롤 없이 보이는지
- [ ] 이메일 링크를 눌렀을 때 메일 앱(또는 메일 작성 창)이 정상적으로 열리는지
- [ ] 시행일이 실제로 배포한 버전과 일치하는지
- [ ] Google Play 콘솔 등에 등록한 URL이 최신 주소로 연결되는지
- [ ] 방침 내용이 앱의 실제 동작(권한 사용, 로컬 저장, 캘린더 예외 설명 등)과
      계속 일치하는지, 앱 기능이 바뀔 때마다 함께 검토
