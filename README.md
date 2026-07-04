# Dragon Fortune Deluxe — 배포 패키지

## 폴더 내용
- index.html — 게임 본체 (v4.1)
- manifest.json / sw.js / icons/ — PWA 필수 요소
- privacy.html — 개인정보처리방침 (이메일 주소 채워넣기!)
- .well-known/assetlinks.json — PWABuilder 지문 받은 뒤 교체

## 순서
1. GitHub에 새 저장소 `dragon-fortune` 생성 → 이 폴더 내용 전부 업로드
2. Settings → Pages → Branch: main → Save
3. https://yyoo316-web.github.io/dragon-fortune/ 접속 확인
4. https://www.pwabuilder.com 에 위 주소 입력 → Package for Stores → Android
   - Package ID: com.lidia.dragonfortune
   - Signing: "Create new" 선택 → 다운로드 zip 안의 signing key 파일은 절대 분실 금지!
5. 다운로드 zip 안의 assetlinks.json 을 .well-known/ 에 덮어쓰고 다시 푸시
6. Play Console → 앱 만들기 → AAB 업로드
   - 콘텐츠 등급 설문: "모의 도박(Simulated Gambling)" 있음 → 성인 등급
   - 데이터 보안: "수집하는 데이터 없음"
   - 개인정보처리방침 URL: https://yyoo316-web.github.io/dragon-fortune/privacy.html
