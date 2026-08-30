# EQ Talk & Game

엘리아 **Extended Learning Question**(Let's Talk!) 말하기 활동용 웹 앱.
HTML 파일 하나로 동작하며 설치·인터넷·서버가 필요 없습니다.

- 교재 **30권 / 3,809문항** (ZOOM 12권 · KEYSTONE 18권)
- 연습 모드 + 게임 4종: **Speed Relay · Flip Cards · Ladder Game · Word Builder**
- 스마트칠판 터치 기준으로 설계(최소 46px 터치 영역), 원어민 교사가 조작
- 점수·순위·팀 대결 없음. 모두 같은 횟수만큼 말하고 다 함께 칭찬으로 마무리

## 파일

| 파일 | 용도 |
|---|---|
| `EQ Talk & Game.html` | **이것만 열면 끝** (연습 + 게임 4종, 데이터 포함) |
| `games.tmpl.html` | 편집용 원본 틀 (`/*DATA*/` 자리에 데이터가 들어감) |
| `data.json` | 질문 원문 데이터 — **수정 금지** |
| `00_게임_가이드.md` | 교사용 진행 가이드 (한국어 + 영어) |

## 다시 빌드

```bash
python3 -c "d=open('data.json').read();t=open('games.tmpl.html').read();open('EQ Talk & Game.html','w').write(t.replace('/*DATA*/',d))"
```

## 저작권

- 게임 코드·디자인·힌트 문장(START LIKE THIS / SAY MORE)·한국어 뜻: **배성미 (Amy English)**
- **질문 원문과 BI 로고는 엘리아영어 본사 저작물입니다.** 외부 공개·재배포 전 본사 동의가 필요합니다.

© 2026 배성미 · Amy English
