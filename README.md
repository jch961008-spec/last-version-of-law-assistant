# 3천만원 이하 소액사건 이행의 소 소장 자동작성 웹앱 (PWA 아이콘 포함)

스마트폰(iOS/Android)이나 PC(Chrome/Edge)에서 **홈 화면에 추가 / 앱 설치**를 실행하면 **펼쳐진 법전 아이콘**이 바탕화면에 생성되도록 PWA(Progressive Web App) 설정이 완료된 패키지입니다.

## 포함된 파일 구성
- `index.html`: 소장 자동작성 웹앱 본체 (PWA 메타태그 및 서비스워커 등록 코드 포함)
- `manifest.json`: 웹앱 이름(`소액소장작성`), 시작 URL, 펼쳐진 법전 아이콘 경로 정의 파일
- `sw.js`: 앱 설치 배너 활성화 및 오프라인 캐시를 지원하는 서비스 워커
- `icon-512.png` / `icon-192.png`: Android 및 PC(Chrome/Edge) 설치용 펼쳐진 법전 아이콘
- `apple-touch-icon.png` (180×180): iPhone / iPad(Safari) 홈 화면 추가용 펼쳐진 법전 아이콘
- `favicon.png`: 브라우저 탭 파비콘
- `.nojekyll` & `.github/workflows/deploy.yml`: GitHub Pages 자동 배포 설정

## GitHub Pages 배포 및 앱 설치 방법
1. GitHub 저장소 루트(`/`)에 이 압축 파일의 모든 파일을 그대로 업로드(Push)합니다.
2. 저장소 **Settings → Pages**에서 `main` 브랜치(또는 GitHub Actions)로 배포를 활성화합니다.
3. 배포된 `https://<계정명>.github.io/<저장소명>/` 주소에 접속합니다.
   - **Android / PC (Chrome · Edge)**: 주소창 오른쪽의 **[앱 설치]** 아이콘(또는 메뉴의 **[홈 화면에 추가 / 앱 설치]**)을 클릭하면 펼쳐진 법전 아이콘으로 설치됩니다.
   - **iPhone / iPad (Safari)**: 하단 **[공유]** 버튼을 누른 뒤 **[홈 화면에 추가]**를 누르면 펼쳐진 법전 아이콘이 홈 화면에 생성됩니다.
