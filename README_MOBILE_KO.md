# GoldBridge 모바일 앱 설치 패키지 (PWA)

## 현재 상태
- 모바일 화면용 웹 앱 소스와 PWA manifest/service worker 포함
- 홈 화면 설치를 위한 아이콘 포함
- 실제 설치 링크(URL)는 아직 게시되지 않음

## PC 없이 게시하는 흐름
1. GitHub 계정 생성/로그인
2. 새 저장소 `goldbridge-mobile` 생성
3. 이 폴더의 모든 파일을 저장소 루트에 업로드
4. Settings → Pages → Deploy from a branch → `main` / `/ (root)` 선택 후 Save
5. GitHub Pages URL이 활성화될 때까지 기다림
6. 갤럭시 Chrome에서 HTTPS URL 열기 → ⋮ → '앱 설치' 또는 '홈 화면에 추가'

## 중요한 제약
- GitHub Pages 게시/계정 설정은 사용자가 직접 수행해야 함. 이 패키지는 자동으로 인터넷에 게시되지 않음.
- PWA는 설치형 웹 앱이지 네이티브 APK가 아님.
- 국제 금 시세 API는 네트워크, CORS, 공급자 정책/제한에 따라 실패할 수 있음.
- 무료 시세는 최대 15분 지연 가능성이 있으므로 '실시간 보장'으로 간주하면 안 됨.
