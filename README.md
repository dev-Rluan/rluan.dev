# rluan.dev

개발자 rluan의 개인 허브. 만든 것, 참여한 프로젝트, 개발 도구, 연락처를 모아 둔다.

디자인: Pebble Village의 밤 캠프를 가져온 픽셀 작업실. 만든 것은 "인벤토리", 지금 하는 일은 "진행 중인 퀘스트", 기술은 "장비", 연락은 "우편함". 글꼴은 Galmuri11(픽셀)과 Pretendard를 jsDelivr에서 불러온다.

- 페이지: `public/` (정적 HTML, 빌드 없음)
- 배포: Cloudflare Workers 정적 자산 (`wrangler.jsonc`)
  - Deploy command: `npx wrangler deploy`
  - 미리보기(PR) 빌드는 `npx wrangler preview`를 쓰므로 `wrangler.jsonc`에 `"previews": {}`가 있어야 한다.
  - Cloudflare 프로젝트 이름은 `wrangler.jsonc`의 `name`(`rluan-dev`)과 같아야 한다.

## 관련 프로젝트

| 프로젝트 | 주소 | 비고 |
|---|---|---|
| Pebblecraft | https://pebblecraft.io | 게임 공방 (Touch Down, Castaways, Massive Consumer) |
| Pebble Village | https://github.com/dev-Rluan/pebble-village | Claude Code·Codex 작업 상태를 보여 주는 로컬 대시보드 (오픈소스) |
| AI Notes | 비공개 | 발표·회의 녹음 받아쓰기·요약 개인 도구. 화면 이미지는 저장소의 `design/previews` 시안 |
| MapleTactics | https://maplestoryworlds.nexon.com/ko/play/d153fb40635e411ea9aa54d2740892a1 (코드: https://github.com/MagunMadown/MapleTactics) | 팀 참여: 전투 시스템, 데이터 검증, 설계 문서 |
| growtok | 준비 중 | 보육일지 작성·관리 서비스 |

## 검색 노출

- 대표 주소(canonical) `https://rluan.dev/`, 공유 미리보기 `public/og.jpg`(1200x630, 첫 화면 장면), 구조화 데이터(Person·WebSite)는 `public/index.html` `<head>`에 있다.
- `public/robots.txt`, `public/sitemap.xml`. 페이지를 추가하면 sitemap에도 넣는다.

## 손으로 고칠 것

- 첫 화면 "진행 중인 퀘스트" 줄: 지금 하는 일로 바꾼다.
- 만든 것을 추가하면 인벤토리 카드를 하나 더 넣고, 화면 이미지는 `public/img/`에 WebP로 둔다.
- 도구(`/qr`, `/crypto`)를 만들면 `public/qr.html` 등으로 넣고 상태를 "준비 중"에서 바꾼다.
