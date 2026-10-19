# 보물상자 — eetoy.github.io 시각화 페이지 로컬 사본

- 배포: gh api PUT (git push 차단 환경) → https://eetoy.github.io/
- index.html = Dr. Dolmaro의 보물상자 메인 (2026-08-11 신설)
- tetraplegia_tendon_reconstruction.html = ICSHT 건이전 가이드 (ASSH Handthology 기반)
- tetraplegia_stroke_note.html = Handthology "Tetraplegia and Stroke" 한글 학습 노트 (2026-08-31, 정본은 `02_문헌정보팀/Tetraplegia_상지재건_노트.html` — 배포본은 noindex 추가, 그림은 ASSH 서버 원본 참조·복제 없음)
- druj_injury_reconstruction_note.html = Handthology "DRUJ Injury and Reconstruction" 한글 학습 노트 (2026-09-08, 정본 `02_문헌정보팀/DRUJ_손상재건_노트.html`, 동일 방식)
- ※ 상시 규칙(2026-09-08 대표): `/handthology` 노트는 완성 시 항상 여기에도 배포 + 카드 추가
- 주 1회(주간 리뷰) 저장소 스캔해 새 html을 메인에 연결 — AI_COMPANY_ROUTINE.md D-4
- median_nerve_compression_note.html = Handthology "Median Nerve Compression" 한글 학습 노트 (2026-09-14, 정본 `02_문헌정보팀/정중신경압박_노트.html`, 동일 방식)

- dropboy/ = dropboy 앱 소개 페이지(Tesla 스타일) + 다운로드 zip (2026-10-19, 원본 앱은 `11_앱개발팀/파일변환앱/`). 앱 새 버전 빌드 시 `ditto -c -k --keepParent dropboy.app dropboy/dropboy.zip` 후 `python3 deploy.py dropboy/dropboy.zip dropboy/index.html`로 재배포
- deploy.py = gh api PUT 배포 스크립트 (인자로 준 파일들을 같은 상대경로로 eetoy.github.io에 올림, 기존 파일은 sha 받아 갱신)
