# Electron-React Todo App

이 프로젝트는 Electron과 React를 사용하여 만든 간단한 투두 애플리케이션입니다. 이 애플리케이션은 TypeScript를 사용하여 작성되었으며, Webpack을 통해 빌드됩니다.

## 목차

- [기능](#기능)
- [시작하기](#시작하기)
  - [필수 조건](#필수-조건)
  - [설치](#설치)
- [애플리케이션 실행](#애플리케이션-실행)
- [폴더 구조](#폴더-구조)
- [스크립트](#스크립트)
- [라이선스](#라이선스)

## 기능

- 새로운 할 일 추가
- 할 일 목록 보기

## 시작하기

### 필수 조건

- node v20.11.1

### 설치

1. 레포지토리를 클론합니다:

```bash
$ git clone https://github.com/lcgyung/study-electron-react-todo.git
$ cd study-electron-react-todo
```

2. 의존성을 설치합니다.

```bash
$ yarn
```

3. 애플리케이션 실행

```bash
$ yarn start
```

## 폴더 구조

```
electron-react-todo/
├── src/
│   ├── main/
│   │   └── main.ts
│   ├── preload/
│   │   └── preload.ts
│   ├── renderer/
│   │   ├── App.tsx
│   │   ├── index.html
│   │   └── index.tsx
├── package.json
├── tsconfig.json
├── webpack.main.config.js
├── webpack.renderer.config.js
├── .gitignore
├── LICENSE
├── dist/
│   ├── main.js
│   ├── renderer.js
│   └── index.html
```

- dist/: 빌드된 파일들이 위치한 디렉터리.
- src/: 소스 파일들이 위치한 디렉터리.
  - main/: Electron 메인 프로세스 파일들이 위치한 디렉터리.
  - preload/: Electron의 preload 스크립트 파일들이 위치한 디렉터리.
  - renderer/: React 렌더러 프로세스 파일들이 위치한 디렉터리.
- webpack.main.config.js: 메인 프로세스를 위한 Webpack 설정 파일.
- webpack.renderer.config.js: 렌더러 프로세스를 위한 Webpack 설정 파일.
