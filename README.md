# Stash 공유 뷰어 (정적 페이지)

- 받는 사람이 여는 공유 링크 화면입니다.
  - 새 링크(v2): `https://bizforbiz.github.io/s/#<m.json 파일 ID>` — 공유 목록(`m.json`)과 원본을 Google Drive API에서 **직접** 읽습니다(Apps Script 안 거침).
  - 옛 링크(v1): `https://bizforbiz.github.io/s/#<공유ID 10자>` — Apps Script 서버(`share-server/Code.gs`의 `vOpen`/`vFile`)에서 받습니다.
- GitHub 저장소 `bizforbiz/s`는 **공개**이며 이 `index.html` 하나만 들어 있습니다. 공유 내용·사진은 없습니다.
  들어 있는 것은 서버 주소(`API_URL`)와 Drive API 키(`DRIVE_API_KEY` — 웹사이트·Drive API로 제한한 공개용 키, `share-server/SETUP.md` 7번)뿐입니다.
- 업데이트: 이 폴더의 `index.html`을 `bizforbiz/s` 저장소 루트에 그대로 복사 → `DRIVE_API_KEY` 값이 들어 있는지 확인 → 커밋 → push (GitHub Pages가 1~2분 뒤 자동 반영).
- Apps Script를 "새 배포"로 다시 만들어 `/exec` 주소가 바뀌면 `index.html` 안의 `API_URL`도 새 주소로 고친 뒤 위처럼 push 하세요.
