FATE — 카드 일러스트 교체 가이드
=======================================

이 폴더(assets/img/)에 카드용 그림을 넣고, index.html 에서 카드에 연결하면
지금의 그라데이션 플레이스홀더가 실제 일러스트로 바뀝니다.

[1] 그림 준비
- 비율: 세로형 3:4 (예: 750 x 1000 px ~ 900 x 1200 px)
- 형식: jpg 또는 png (용량은 한 장당 300KB 이하 권장 → 로딩 빠름)
- 파일명: 영어/숫자로 (예: love1.jpg, wealth1.jpg). 한글·공백 피하기.

[2] 폴더에 넣기
- 이 폴더(assets/img/)에 그림 파일을 복사해 넣습니다.
  예) assets/img/love1.jpg

[3] index.html 에서 카드에 연결
- 바꾸고 싶은 카드 한 줄을 찾습니다. 예:
  <div class="pcard g-love" data-cat="love" onclick="comingSoon()">
    <div class="motif">💘</div><h4 ...>2026 연애운 사주</h4><span ...>...</span></div>

- 여기서 두 가지만 바꾸면 됩니다:
  (1) class 에 has-img 추가
  (2) style 로 배경 이미지 지정

  바꾼 결과:
  <div class="pcard g-love has-img" data-cat="love"
       style="background-image:url('assets/img/love1.jpg')" onclick="comingSoon()">
    <div class="motif">💘</div><h4 ...>2026 연애운 사주</h4><span ...>...</span></div>

  → 이모지(motif)는 자동으로 숨겨지고, 그림 위에 제목이 읽기 좋게 표시됩니다.

[4] 히어로(큰 카드)도 동일
  <div class="hcard g-fortune has-img"
       style="background-image:url('assets/img/hero1.jpg')" onclick="openTool('today')"> ...

[5] 저작권 주의
- 반드시 "직접 만든 그림" 또는 "상업적 사용 허가된 그림"만 사용하세요.
- 다른 앱/사이트의 그림을 그대로 쓰면 안 됩니다.
- AI로 생성한 그림을 쓸 경우, 해당 서비스의 상업적 이용 약관을 확인하세요.

[참고] 그림 만드는 방법 (택1)
- 디자이너에게 의뢰 / 크몽·미리캔버스 등
- 유료 AI 이미지 생성(Midjourney, DALL·E 등) — 상업적 이용 가능 플랜
- 무료 일러스트 사이트(unDraw 등) — 단, 웹툰풍은 아님

도움이 필요하면 "이미지 넣어줘"라고 말씀하시면 연결해 드립니다.
