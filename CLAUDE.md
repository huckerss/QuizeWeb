# CLAUDE.md

This file provides guidance to Claude Code (claude.ai/code) when working with code in this repository.

## Project Overview

QuizeWeb is a browser-based quiz web application. It uses a minimal Express.js server to serve static files, deployed on Railway.

## Development

```bash
# 의존성 설치
npm install

# 서버 실행 (localhost:3000)
npm start
```

## Deployment (Railway)

Railway는 `package.json`의 `start` 스크립트를 자동으로 감지합니다.
`PORT` 환경변수는 Railway가 자동으로 주입합니다.

## Architecture

- `server.js` — Express 정적 파일 서버. `public/` 폴더를 서빙하며 모든 경로를 `index.html`로 라우팅
- `public/` — 모든 정적 파일 (HTML, CSS, JS) 위치
- `public/index.html` — 앱 진입점
