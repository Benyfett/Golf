# 골프

개인용 골프 웹앱 모음. GitHub Pages로 배포됩니다.

- 모음 페이지: https://benyfett.github.io/Golf/
- 스윙 프레임: https://benyfett.github.io/Golf/swing-frame/

## 구조
- `index.html` — 앱 목록 페이지 (서비스 워커 없음: 하위 앱을 가로채지 않도록)
- `swing-frame/` — 스윙 영상 프레임 분석 앱. 오프라인 캐시(`sw.js`)는 이 폴더 안에서만 동작

## 새 앱 추가 원칙
- 앱마다 자기 폴더 하나. 다른 폴더 파일은 건드리지 않는다.
- 서비스 워커·매니페스트는 각 앱 폴더 안에 두어 범위를 그 폴더로 한정한다.
- 브라우저 저장 키는 앱 이름으로 시작하게 해서 다른 앱과 겹치지 않게 한다 (예: `swingframe.settings.v1`).
- 저장소는 공개이므로 개인·회사 데이터는 코드에 넣지 않는다.
