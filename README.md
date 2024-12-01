# Todolist, react
https://lee2567.github.io/ReactTodolist4/

 공식 문서 : https://create-react-app.dev/docs/deployment/#github-pages

 에러 : github page 업로드가 안됌, page가 빈 화면으로 나타남, 경로를 못 찾음

시도:

--------------------------------------------------------------------

  "dependencies": 
  "react-beautiful-dnd": "^13.1.1",
  "react-dom": "^18.3.1",
   "react-router": "^7.0.1",
  "react-router-dom": "^7.0.1",
  "web-vitals": "^2.1.4",
--------------------------------------------------------------------

    "scripts":
    "start": "react-scripts start",
    "build": "react-scripts build",
    "predeploy": "npm run build",
    "deploy": "gh-pages -d build",
    "build:staging": "env-cmd -f .env.staging npm run build"
--------------------------------------------------------------------
    "homepage": "."
    
  핵심 해결 방안
  1. react 공식문서를 따라 진행한다
  2. build 파일만 업로드 한다 (todolist는 단일페이지이다)
  3. github 업로드에 git모듈이 충돌하지 않게 깃허브앱 연동 파일을 분리한다
