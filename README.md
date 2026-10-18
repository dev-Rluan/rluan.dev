# rluan.dev

개발자 rluan의 개인 허브. 만든 것, 참여한 프로젝트, 개발 도구, 연락처를 모아 둔다.

- 페이지: `public/` (정적 HTML, 빌드 없음)
- 배포: Cloudflare Workers 정적 자산 (`wrangler.jsonc`)
  - Deploy command: `npx wrangler deploy`
  - Preview command: `npx wrangler versions upload`
  - Cloudflare 프로젝트 이름은 `wrangler.jsonc`의 `name`(`rluan-dev`)과 같아야 한다.

## 관련 프로젝트

| 프로젝트 | 주소 | 비고 |
|---|---|---|
| Pebblecraft | https://pebblecraft.io | 게임 공방 (Touch Down, Castaways, Massive Consumer) |
| MapleTactics | https://github.com/MagunMadown/MapleTactics | 팀 참여: 전투 시스템, 데이터 검증, 설계 문서 |
| growtok | 준비 중 | 보육일지 작성·관리 서비스 |

## 손으로 고칠 것

- 첫 화면 `NOW` 줄: 지금 하는 일로 바꾼다.
- 도구(`/qr`, `/crypto`)를 만들면 `public/qr.html` 등으로 넣고 상태를 "준비 중"에서 바꾼다.
