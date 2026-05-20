# 온라인 공유/배포 방법

이 폴더는 정적 HTML 사이트입니다. `index.html`이 메인 페이지이므로 Vercel, Netlify, GitHub Pages 어디에 올려도 바로 열립니다.

## 추천: Vercel

### 1. GitHub 저장소로 연결하는 방법

1. 이 폴더를 GitHub 저장소에 올립니다.
2. Vercel에서 `New Project`를 누르고 해당 저장소를 Import합니다.
3. Framework Preset은 `Other` 또는 자동 감지 그대로 둡니다.
4. Build Command는 비워둡니다.
5. Output Directory도 비워두거나 `.`로 둡니다.
6. Deploy를 누릅니다.

이후 `index.html`, `sg_ai_contest_ideas.md`, `sg_ai_contest_ideas.html`을 수정해서 GitHub에 push하면 Vercel이 자동으로 다시 배포합니다.

### 2. Vercel CLI로 바로 배포하는 방법

```powershell
npx vercel
```

첫 실행 시 Vercel 로그인이 필요합니다. 질문이 나오면 대부분 기본값으로 진행하면 됩니다.

운영 URL로 확정 배포하려면:

```powershell
npx vercel --prod
```

## 대안

| 방법 | 장점 | 단점 |
|---|---|---|
| Vercel | 가장 빠르고 깔끔함, 자동 배포 쉬움 | 계정 로그인 필요 |
| GitHub Pages | 무료, 저장소만 있으면 됨 | 설정이 약간 번거로울 수 있음 |
| Netlify | 드래그 앤 드롭 배포가 쉬움 | 계정 필요 |
| 임시 터널(localtunnel/ngrok) | 지금 바로 공유 가능 | PC가 켜져 있고 프로세스가 실행 중이어야 함 |

## 팀 운영 방식 추천

1. 원본 내용은 `sg_ai_contest_ideas.md`에서 관리합니다.
2. 공유용 화면은 `index.html`과 `sg_ai_contest_ideas.html`을 업데이트합니다.
3. GitHub에 push하면 Vercel 배포 링크가 자동 업데이트되도록 만듭니다.

