# spotalarm-link

SpotAlarm(`com.mindstartium.spotalarm`) 공유 링크 `https://spotalarm.mindstartium.com/c#<코드>` 받기 페이지.
GitHub Pages + Cloudflare DNS(CNAME `spotalarm` → `moyuchan84.github.io`, DNS only).

| 파일 | 역할 |
| --- | --- |
| `c.html` | 받기 페이지. 카카오톡 등 인앱 브라우저에서 `intent://` 로 앱을 연다. 카드 내용은 `#` 뒤에만 있어 서버로 가지 않는다 |
| `.well-known/assetlinks.json` | Android 앱 링크 검증. 업로드 키·debug 키 SHA-256. Play 앱 서명 키는 앱 등록 후 추가 |
| `og.png` | 카카오톡·문자 링크 미리보기 이미지 |
| `index.html` | 루트 안내 |
| `.nojekyll` | `.well-known` 폴더를 그대로 배포하려고 Jekyll을 끈다 |
