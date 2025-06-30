# 프로젝트 구조 설명서 (THREED)

이 문서는 `THREED` 프로젝트의 기본 폴더 구조 및 주요 파일의 역할에 대해 설명합니다.

## 루트 디렉터리 구조
THREED/
├── .next/ # Next.js에서 자동 생성되는 빌드 결과물
├── node_modules/ # 설치된 NPM 패키지
├── public/ # 정적 파일 (이미지, 폰트 등)
├── src/ # 실제 프로젝트 소스 코드 폴더
├── .gitignore
├── next-env.d.ts # TypeScript용 Next.js 환경 타입 선언
├── eslint.config.mjs # 린트 설정
├── tsconfig.json # TypeScript 설정

page
├──home
├──├──components
├──├──constants
├──├──hooks
├──├──home.component.tsx
├──├──home.module.scss

```



---

## `public/`

- `images/` — 프로젝트에서 사용하는 정적 이미지 리소스
- `fonts/` — 웹폰트가 있을 경우 이곳에 저장

> 이 경로의 파일은 브라우저에서 `/images/파일명` 형식으로 접근할 수 있습니다.

---

## `src/`

### `app/`

- Next.js 13 이상의 App Router 기능을 사용하며, `page.tsx` 기반의 라우팅 구성
- `/login`, `/post` 등의 폴더가 각각의 페이지 라우트를 의미합니다.

> 예:
> - `/login/page.tsx` → `도메인.com/login`
> - `/post/page.tsx` → `도메인.com/post`

## 개발 환경 설정

## 필요한 도구

- Node.js (권장: 18 이상)
- yarn 설치
```javascript
npm install -g yarn
```

## 패키지 설치


yarn install

## 개발 서버 실행
yarn dev
url : http://localhost:3000

## 프로젝트 빌드
yarn run build

## 빌드 후 실행
yarn run start

## 코드 정리 및 검사
yarn run lint
