

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


## 대표 가수 카테고리 정규화 보강

다음 표기는 하나의 카테고리로 통일됩니다.

```text
Choi Yu Ree / Choi Yuri / Yu Ree Choi → 최유리
Sung Si Kyung / Sung Si-kyung / Sung Sikyung → 성시경
Kim Jong Kook / Kim Jong-kook / Jong Kook Kim / 종국김 → 김종국
Lee Mu Jin / LEE MU JIN / 리무진서비스 → 이무진
Roy Kim → 로이킴
BOL4 / Bolbbalgan4 / 안지영 → 볼빨간사춘기
BIG Naughty / 빅나티 / 서동현 → BIG Naughty
JANNABI → 잔나비
JONGHYUN → 종현
KYUHYUN → 규현
PLAVE / 플레이브 → PLAVE
Akdong Musician / 악동뮤지션 / 이찬혁 / 이수현 → AKMU
```

또한 대표 가수 카테고리에 해당하는 항목은 곡 수가 1~2개여도 `기타`로 이동하지 않습니다.


## 추가 카테고리 정리

다음 항목을 보정했습니다.

```text
Jason Mraz → Jason Mraz 카테고리
𝐋𝐀𝐍𝐘 / LANY / lany → LANY 카테고리
Charlie Puth / Charlie Puth (찰리 푸스) → 찰리푸스 카테고리
Sung Si Kyung / Sung Si-kyung / Sung Sikyung → 성시경 카테고리
```

특히 `기타`로 빠지던 LANY와 Jason Mraz는 대표 카테고리로 고정되며, 성시경은 영어 표기 대신 한국어 카테고리명으로 통일됩니다.
