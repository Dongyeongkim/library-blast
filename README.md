# 목소리로 도서관 폭파

목소리(크기 + 공명 음높이)만으로 POSTECH · KAIST · UNIST · DGIST 도서관을 무너뜨리는 3D 시뮬레이터.

- 말러 교향곡 2번 「부활」 5악장 마지막 합창 30초("Aufersteh'n, ja aufersteh'n wirst du, mein Herz, in einem Nu!")를 따라 부르면 음을 맞힌 음절마다 유리가 깨지고 진동이 쌓여 무너집니다.
- 선율은 1897년 Hofmeister 초판 총보(퍼블릭 도메인, 인터넷 아카이브 `symphonieno200mahl`) 204쪽 연습번호 48의 소프라노 파트에서 옮겼습니다. 한두 옥타브 아래로 불러도 됩니다.
- 혼자 모드 / 스크리밍 데이(여럿이 함께) 모드
- WASD 이동, Space 점프, 드래그로 회전, 스크롤로 확대

three.js 0.160 하나만 CDN으로 불러오는 단일 `index.html`입니다. 아무 정적 서버로나 열 수 있습니다.

```bash
python3 -m http.server 4211
```
