# 목소리로 도서관 폭파

목소리(크기 + 공명 음높이)만으로 POSTECH · KAIST · UNIST · DGIST 도서관을 무너뜨리는 3D 시뮬레이터.

- 마이크 권한을 허용하고 건물의 공명 음높이에 맞춰 외치면 금이 가고 무너집니다.
- 말러 합창 모드: 번스타인·런던 심포니 녹음(유튜브 공식 퍼가기 플레이어, FZEusNJLoRw)을 틀어 놓고 교향곡 2번 「부활」의 마지막 합창("werde ich entschweben … zu Gott wird es dich tragen!")을 같이 부릅니다. 가사가 화면에 뜨고, 아래 노래방식 음정 띠에서 음표 위치와 내 음을 볼 수 있습니다. 유튜브를 못 불러오면 합성 가이드 노래로 대신합니다.
- "Aufersteh'n…" 구간 음은 1897년 Hofmeister 초판 총보(퍼블릭 도메인, 인터넷 아카이브 `symphonieno200mahl`) 204쪽 연습번호 48의 소프라노 파트에서 옮겨 녹음 시각에 맞췄고, 47번 "Sterben werd' ich" 두 번(203쪽)도 같은 총보에서 옮겼습니다. 맨 앞 "werde ich entschweben"과 끝 "Was du geschlagen…"은 음표 없이 가사만 띄웁니다. 한두 옥타브 아래로 불러도 됩니다.
- 혼자 모드 / 스크리밍 데이(여럿이 함께) 모드 / 말러 합창 모드 / 1812 서곡 가면 축제 모드 / 제국 찬가 모드
- WASD 이동, Space 점프, 드래그로 회전, 스크롤로 확대

three.js 0.160 하나만 CDN으로 불러오는 단일 `index.html`입니다. 아무 정적 서버로나 열 수 있습니다.

```bash
python3 -m http.server 4211
```

## 1812 서곡 가면 축제 모드

차이콥스키 「1812년 서곡」 피날레가 흐르는 동안 가면을 쓴 학생들과 함께 외칩니다. 대포가 터지는 순간 크게 외치면 명중해 건물이 크게 부서지고, 무너지면 모두 광장으로 나와 불꽃놀이를 봅니다.

- 음원: `audio/1812-finale.m4a` — Tchaikovsky, *1812 Overture*, "The President's Own" United States Marine Band, 2019년 5월 26일 울프트랩 연주. 미국 정부 저작물이라 퍼블릭 도메인 ([위키미디어 공용](https://commons.wikimedia.org/wiki/File:1812_Overture_-_United_States_Marine_Band.opus)). 원본 650~731초를 잘라 AAC로 변환.
- 대포 시각은 녹음 음량의 급상승을 분석해 뽑았습니다. 화면 아래 띠에 대포 표시가 흘러와 세로선에 닿는 순간을 보여 줍니다.
- 서곡 앞 37초 인트로: 건물 밖에서 천천히 다가가며 실제 빅벤 녹음이 나옵니다 — 1945년 1월 1일 자정 라디오 오라녜 중계(퍼블릭 도메인, [위키미디어 공용](https://commons.wikimedia.org/wiki/File:Westminster_chimes_(1_January_1945).wav))에서 시보 타종 세 번과 웨스트민스터 차임을 잘라 이은 `audio/bigben-intro.m4a`. 타종 사이에는 유튜브 영상 「Remember Remember the 5th of November - V for Vendetta」(RS2HLC0sipA)의 34초부터 15초를 유튜브 공식 퍼가기 플레이어로 틀어 대사를 들려줍니다(음원을 따로 떼어 넣지 않음). 유튜브를 못 불러오면 영국 전래 동요 「Remember, remember the fifth of November」(퍼블릭 도메인)를 브라우저 음성으로 낭독합니다. "인트로 건너뛰기"로 바로 시작할 수 있고, 영화의 음성·음악은 쓰지 않습니다.
- 가면은 실존 인물 가이 포크스의 캐리커처(흰 얼굴, 말린 콧수염, 뾰족한 턱수염)를 직접 단순하게 만든 것입니다.

## 제국 찬가 모드

오스트리아-헝가리 제국 찬가 「Gott erhalte, Gott beschütze」(하이든 선율 1797, 요한 가브리엘 자이들 가사 1854, 1918년까지 사용) 1절을 따라 부릅니다. 선율은 영어 위키백과 "Gott erhalte Franz den Kaiser" 문서의 악보에서 옮겼고, 합창 소리·오르간 화음·베이스는 브라우저가 직접 합성해 연주합니다(화음은 선율에 맞춰 단순하게 붙인 것으로 하이든의 원래 화성과는 다릅니다).
