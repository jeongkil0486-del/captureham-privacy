# 캡처함 개인정보처리방침 페이지

이 폴더는 캡처함(JG Studio KR) 앱의 **외부 공개용 개인정보처리방침**
정적 웹페이지입니다. 서버, 데이터베이스, JavaScript 없이 `index.html`
하나로 완성된 페이지이며, Google Play 콘솔의 개인정보처리방침 URL
항목이나 앱 스토어 등록에 그대로 사용할 수 있습니다.

## 파일 설명

- `index.html` — 개인정보처리방침 전체 내용을 담은 단일 HTML 파일.
  외부 CSS/JS/폰트/이미지를 전혀 불러오지 않으며, 이 파일 하나만
  열어도 완성된 화면이 표시됩니다.
- `README.md` — 이 문서.

## 브라우저에서 확인하는 방법

1. 파일 탐색기에서 `privacy-policy/index.html`을 더블클릭해 기본
   브라우저로 엽니다.
2. 또는 브라우저 주소창에 파일 경로를 직접 입력해도 됩니다.
   예: `file:///C:/FlutterProjects/capture_assistant/privacy-policy/index.html`
3. 인터넷 연결 없이도 정상적으로 표시되는지 확인해 보세요
   (외부 리소스를 전혀 사용하지 않기 때문에 오프라인에서도 동일하게 보입니다).

## GitHub Pages에 공개하는 방법

아래 절차는 안내만 담고 있으며, 이 작업에서 실제로 Git push나
GitHub Pages 설정을 실행하지는 않았습니다. 준비가 되면 직접
진행해 주세요.

1. GitHub에 새 저장소를 만들거나(예: `capture-assistant-privacy`),
   기존 프로젝트 저장소를 사용합니다.
2. 이 `privacy-policy` 폴더의 내용을 저장소에 커밋하고 GitHub에
   push합니다.
   - 별도 저장소를 쓰는 경우: `privacy-policy` 폴더 안의 파일들을
     저장소 루트로 복사해서 올리면 URL이 더 짧아집니다.
   - 기존 프로젝트 저장소를 그대로 쓰는 경우: 폴더 구조를 유지한 채
     올려도 됩니다.
3. GitHub 저장소 페이지에서 **Settings → Pages**로 이동합니다.
4. **Build and deployment** 항목에서 배포할 브랜치(예: `main`)와
   폴더를 선택합니다.
   - 폴더를 저장소 루트로 옮겼다면 `/ (root)`를 선택하세요.
   - `privacy-policy` 폴더를 그대로 두었다면, 저장소 루트에 있는
     `index.html`이 없으므로 별도 저장소를 만들거나 루트로 복사하는
     방식을 권장합니다(GitHub Pages는 기본적으로 저장소 루트 또는
     `/docs` 폴더만 지원합니다).
5. 저장 후 몇 분 뒤 GitHub가 안내하는 주소
   (예: `https://내계정.github.io/저장소이름/`)로 접속해 페이지가
   정상적으로 보이는지 확인합니다.
6. 이 URL을 Google Play 콘솔의 "개인정보처리방침" 항목이나 앱스토어
   등록 정보에 입력합니다.

## 시행일 수정 위치

`index.html`의 `<header>` 안, 다음 줄을 찾아 날짜를 바꿉니다.

```html
<span class="effective-date">
  최초 시행일: 2026년 7월 24일 · 개정 및 시행일: 2026년 8월 11일
</span>
```

방침 내용을 실제로 변경했을 때만 이 날짜를 갱신하세요.

## 개발자명과 이메일 수정 위치

`index.html`의 "제13조 문의처" 섹션, `contact-box` 안에 있습니다.

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
