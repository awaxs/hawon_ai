1. pakage.json 에 gh-pages 설치

아래 명령을 실행 하면
      npm i gh-pages -D

  },
  "devDependencies": {
    "gh-pages": "^6.0.0"
  }

  package.json에 설치되어진게 보인다

  2. package.json 안에 homepage 작성
      "homepage": "https://아이디.github.io/리포지토리이름",
      아래 처럼
  {
  "name": "awaxs-github-io-hawon_ai",
  "version": "0.1.0",
  "private": true,
  "homepage": "https://awaxs.github.io/hawon_ai",
  "dependencies": {

3. package.json에서 script 에 "deploy": "gh-pages -d build" 가 있는지 확인

  "scripts": {
    "start": "react-scripts start",
    "build": "react-scripts build",
    "test": "react-scripts test",
    "eject": "react-scripts eject",
    "predeploy": "npm run build",
    "deploy": "gh-pages -d build"
  },
4. git init 실행
      내 project 폴더에 git 폴더를 만든다.

5. github 에 repository 를 만든다 
      git push
      git add .
      git commit -m "first commit"
      git remote add origin https://github.com/awaxs/hawon_ai.git
      git branch -M main
      git push -u origin main

6. npm run build  
      Published가 완료 되면 build 가 만들어진다.

7. github 접속하여 