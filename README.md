# HaBong 포트폴리오

https://habong96.github.io — 직접 기획하고 만든 도트 게임을 브라우저에서 바로 플레이할 수 있는 사이트.

## 구조

| 경로 | 내용 |
|---|---|
| `index.html` | 첫 화면: 소개 · 게임 · 기획서 · 게임 분석 · 영상 · 후원 |
| `assets/site.css` | 사이트 전체 모양 (게임 속 도트 UI와 같은 색 · 테두리) |
| `assets/fonts/` | 제목용 도트 글꼴 Galmuri11 (OFL) |
| `games/<게임>/index.html` | 게임 소개 페이지 (플레이 · 기획 포인트 · 만든 과정 · 스크린샷) |
| `games/<게임>/play/` | Godot 웹 빌드 (직접 고치지 않음, 게임 저장소의 스크립트가 넣음) |
| `games/<게임>/img/` | 소개 그림 (게임 저장소의 스크립트가 넣음) |

## 게임 올리기

- 픽셀런 다이노: 게임 저장소(PixelRun)에서 `python tools/publish_site.py --godot <Godot 4.7.2 경로>` → 이 저장소에서 커밋 · 푸시
- 새 게임: `games/<새 게임>/`을 만들고 `index.html` 게임 카드에 한 장 추가

## 미리 보기

```
python -m http.server 8766
```

→ http://localhost:8766
