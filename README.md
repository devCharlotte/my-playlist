

### 링크 추가

`links.txt`에 YouTube 링크를 콤마 또는 줄바꿈으로 추가하기
PR도 가능!!!

```text
https://www.youtube.com/watch?v=VIDEO_ID,
https://youtu.be/VIDEO_ID,
https://www.youtube.com/playlist?list=PLAYLIST_ID
```

### 대표 가수 카테고리

자동 분류에서 우선 카테고리로 고정되는 가수들
```text
최유리, 로이킴, Charlie Puth, Lauv, LANY, Peder Elias, Ed Sheeran,
이무진, 성시경, 규현, Bruno Mars, 볼빨간사춘기, 카더가든, 종현,
잔나비, 10CM, BIG Naughty, AKMU, Crush, 다비치, PLAVE,
Pink Sweat$, 폴킴, DAY6, 김종국, 멜로망스 등
```
곡 수가 1~2개인 가수는 `기타`로 배치

## 기능
- 팝송 / 한국 노래 자동 분류
- 대표 가수 이름별 카테고리 자동 생성
- 기타 카테고리 자동 생성
- 카테고리별 재생
- 카테고리별 랜덤 재생
- 카테고리별 셔플 큐
- 영상 종료 시 자동 다음 항목 재생
- YouTube oEmbed 기반 제목/채널/썸네일 자동 수집


## 제목 표시 개선

`watch?v=...&list=RD...`처럼 추천/라디오 playlist 파라미터가 붙은 YouTube 링크도 곡 영상으로 우선 처리합니다.
카드 제목은 가능한 경우 `가수 - 제목` 형식으로 표시됩니다.

## 수동 보정 규칙

다음 항목은 제목/가수 분류가 어긋나지 않도록 수동 보정 규칙을 추가했습니다.

- 종국김 → 김종국
- 딘딘/DINDIN → 딘딘, 제목은 `인생네컷`
- Black Skirts/블랙스커트 → 검정치마
- 방예담/BANG YEDAM → 비긴어게인 방예담
- One Direction, Coldplay 카테고리 추가
- Stephen Sanchez - Until I Found You
- The Rare Occasions - Notion
- Jin Ah Kwon/권진아 - 운이 좋았지
- 안지영 → 볼빨간사춘기
- 백아, 백예린 카테고리 추가
- 그랬나봐 → 카더가든


## 추가 보정 규칙

- Oasis 카테고리를 추가했습니다.
- `cmpRLQZkTb8`은 Oasis - Don't Look Back In Anger로 처리합니다.
- `vIPug7A8Fds`는 규현으로 처리합니다.
- `ROIvbbg8jMQ`, `4FvqdZtH4xo`, `-RqRdRoEzJo`, `ZsuX9aSst-4`, `znKyb6OOq60`은 잔나비로 처리합니다.
- 최유리 영어 표기와 한국어 표기는 같은 최유리 카테고리로 통일합니다.
- 성시경, 김종국 등 한국 가수의 영문 표기는 한글 카테고리로 통일합니다.
- 이찬혁/이수현은 AKMU로, 안지영/BOL4는 볼빨간사춘기로 통일합니다.
