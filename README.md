# 오늘뭐먹지 AI

냉장고 재료 또는 오늘의 기분과 예산을 바탕으로 메뉴 세 가지를 추천하는 반응형 웹앱입니다.

## 실행

Node.js 18 이상에서 프로젝트 폴더에서 실행하세요.

```bash
npm start
```

브라우저에서 `http://localhost:3000`을 열면 됩니다. Gemini 키가 없어도 기본 메뉴 추천으로 사용할 수 있습니다.

## Gemini AI 연결

`GEMINI_API_KEY` 환경 변수를 지정하고 서버를 실행하면 실제 Gemini 추천을 사용합니다. 키는 브라우저로 전달되지 않습니다.

PowerShell:

```powershell
$env:GEMINI_API_KEY="발급받은_API_키"
npm start
```

## 기능

- 냉장고 파먹기 / 외식·배달 모드
- 재료 태그와 빠른 재료 선택, 조리 도구, 기분·예산 선택
- 메뉴 3개와 조리 순서 또는 주문 팁, 복사, 재추천
- 브라우저 `localStorage` 기반 찜 보관함
- 모바일 반응형 화면
