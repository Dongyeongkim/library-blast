# 목소리로 도서관 폭파

목소리(크기 + 공명 음높이)만으로 POSTECH · KAIST · UNIST · DGIST 도서관을 무너뜨리는 3D 시뮬레이터.

- 마이크 권한을 허용하고 건물의 공명 음높이에 맞춰 외치면 금이 가고 무너집니다.
- 말러 합창 모드: 번스타인·런던 심포니 녹음(유튜브 공식 퍼가기 플레이어, FZEusNJLoRw)을 틀어 놓고 교향곡 2번 「부활」의 마지막 합창("werde ich entschweben … zu Gott wird es dich tragen!")을 같이 부릅니다. 가사가 화면에 뜨고, 아래 노래방식 음정 띠에서 음표 위치와 내 음을 볼 수 있습니다. 유튜브를 못 불러오면 합성 가이드 노래로 대신합니다.
- "Aufersteh'n…" 구간 음은 1897년 Hofmeister 초판 총보(퍼블릭 도메인, 인터넷 아카이브 `symphonieno200mahl`) 204쪽 연습번호 48의 소프라노 파트에서 옮겨 녹음 시각에 맞췄고, 47번 "Sterben werd' ich" 두 번(203쪽)도 같은 총보에서 옮겼습니다. 맨 앞 "werde ich entschweben"과 끝 "Was du geschlagen…"은 음표 없이 가사만 띄웁니다. 한두 옥타브 아래로 불러도 됩니다.
- 혼자 모드 / 스크리밍 데이(여럿이 함께) 모드 / 말러 합창 모드
- WASD 이동, Space 점프, 드래그로 회전, 스크롤로 확대

three.js 0.160 하나만 CDN으로 불러오는 단일 `index.html`입니다. 아무 정적 서버로나 열 수 있습니다.

```bash
python3 -m http.server 4211
```
