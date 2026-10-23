# STRUCTURE · onwha-sample

```
onwha-sample/
├─ index.html              단일 파일 (CSS·JS 인라인)
├─ wrangler.toml           name = onwha-sample → onwha-sample.lgt3232.workers.dev
├─ .assetsignore           img/ · 문서 · index_*.html · _deploy 배포 제외
├─ ow-songmyung.woff2      한글 제목 (송명, 사용 글자만 → 글자 추가 시 재생성)
├─ ow-cormorant.woff2      영문 라벨 (Cormorant Garamond 300–600, 라틴만)
├─ ow-pretendard.woff2     본문 (Pretendard 400–600, 사용 글자만)
├─ ow-logo.webp            로고 먹색 투명 (히어로)
├─ ow-logo-light.webp      로고 밝은색 투명 (해질녘 · 푸터)
├─ ow-*.webp               사진 15장
├─ favicon.png / og-onwha.jpg
├─ img/                    다올 제공 원본 28장 (배포 제외)
└─ CHANGELOG.md / STRUCTURE.md
```

## 섹션 순서
헤더 → 히어로 → `#day` → `#menu`(면 #EFE7DF) → `#yard` → `.dusk-band`(낮→해질녘 그라데이션) → 해질녘 사진 + 맺음말(`.dusk`) → `#visit`(`.dusk`) → 푸터 + 모바일 `.quick`.

## 해질녘 전환
첫 `.dusk` 섹션 위치로 헤더(`.site-head.dark`) · 하단 바(`.quick.dark`) 색을 바꿈. 섹션 순서를 바꾸면 이 기준도 같이 바뀜.

## 영업시간 수정 (4곳)
히어로 `.sub` · Visit `.info` · 푸터 · head JSON-LD.

## 폰트 재생성
문구를 바꾸면 항상 빠진 글자 검사(LESSONS §26). `pyftsubset … --name-IDs='*' --name-languages='*' --name-legacy` (§24).
