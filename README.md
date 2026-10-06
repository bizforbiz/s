# Stash 공유 뷰어 (정적 페이지)

- 받는 사람이 여는 공유 링크 화면입니다: `https://bizforbiz.github.io/s/#<공유ID>` — 데이터는 페이지가 Apps Script 서버(`share-server/Code.gs`의 `vOpen`/`vFile`)에서 직접 받아 옵니다.
- GitHub 저장소 `bizforbiz/s`는 **공개**이며 이 `index.html` 하나만 들어 있습니다. API 키·공유 내용·사진 등 데이터는 전혀 없습니다(서버 주소만 들어 있음).
- 업데이트: 이 폴더의 `index.html`을 `bizforbiz/s` 저장소 루트에 그대로 복사 → 커밋 → push (GitHub Pages가 1~2분 뒤 자동 반영).
- Apps Script를 "새 배포"로 다시 만들어 `/exec` 주소가 바뀌면 `index.html` 안의 `API_URL`도 새 주소로 고친 뒤 위처럼 push 하세요.
