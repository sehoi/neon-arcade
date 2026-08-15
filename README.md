# NEON ARCADE

세 게임을 고르는 허브 페이지.

### ▶ [https://sehoi.github.io/neon-arcade/](https://sehoi.github.io/neon-arcade/)

| 게임 | 장르 | 화면 | 저장소 |
|---|---|---|---|
| [NEON PURGE](https://sehoi.github.io/neon-purge/) | 뱀서라이크, 10분 | 가로 | [sehoi/neon-purge](https://github.com/sehoi/neon-purge) |
| [NEON COIL](https://sehoi.github.io/neon-coil/) | slither.io 계열 | 가로 | [sehoi/neon-coil](https://github.com/sehoi/neon-coil) |
| [NEON FIREWALL](https://sehoi.github.io/neon-firewall/) | 갤러그 계열 고정 슈터 | 세로 | [sehoi/neon-firewall](https://github.com/sehoi/neon-firewall) |

## 구성

`index.html` **한 파일**이 전부다. CSS는 인라인, 게임 썸네일은 손으로 쓴 인라인 SVG —
이미지 파일도, 폰트 파일도, 스크립트도 없다. 세 게임의 "에셋 파일 0개" 원칙을 그대로 따랐다.

`serve.mjs` 는 로컬 확인용 정적 서버다.

```bash
node serve.mjs
```

http://localhost:5176 (`PORT` 환경변수로 바꿀 수 있다)

## 확인한 것

| 폭 | 결과 |
|---|---|
| 1280px | 3열, 카드 높이 균일(372px), 가로 넘침 없음 |
| 375px | 1열, 카드 335px, 가로 넘침 없음 |
| 320px | 1열, 하단 메타가 2줄로 접힘. 잘림·넘침 없음 |

링크 3개 모두 200 응답. 콘솔 오류 없음.

## 왜 별도 저장소인가

`sehoi.github.io` 에는 2021년에 올린 Jekyll 블로그가 이미 들어 있다.
루트를 허브로 쓰면 그 블로그를 덮어쓰게 되므로 건드리지 않았다.
