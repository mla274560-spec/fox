# 섬/대륙 보상표 (데이터형 웹페이지)

## 1) 수정은 어디를?
- **data.json**만 수정하면 됩니다.
- 섬/대륙 추가/삭제/수정: `locations` 배열을 편집
- 보상 추가/삭제/수정: 각 location의 `rewards` 배열을 편집

## 2) 로컬에서 여는 방법 (중요)
브라우저는 보안 때문에 `file://`로 열면 JSON 로드를 막는 경우가 있습니다.
아래 중 하나로 열면 100% 정상 동작합니다.

### 방법 A: 파이썬 (가장 간단)
1) 이 폴더에서 터미널 열기
2) 실행:
   - Windows: `python -m http.server 8000`
3) 브라우저에서 열기:
   - `http://localhost:8000`

### 방법 B: VS Code Live Server
1) VS Code 설치
2) 확장: **Live Server** 설치
3) `index.html` 우클릭 → **Open with Live Server**

## 3) 이미지(아이콘) 교체
- `assets/` 폴더에 이미지 넣고
- data.json에서 `icon` 값을 예: `assets/라비온.png` 처럼 바꾸면 됩니다.

## 4) 배포(링크 공유) 추천
- GitHub Pages / Netlify / Vercel에 올리면 디스코드에 링크로 공유 가능


## 5) 목차 썸네일
- 목차에 표시되는 이미지는 `assets/thumbs/`의 정사각 썸네일을 사용합니다.
- 새 이미지로 바꾸면 동일하게 썸네일을 만들고 data.json의 `icon` 경로를 업데이트하세요.
