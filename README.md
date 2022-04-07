# Nuxt-basics

- **서버 사이드 렌더링**: 서버에서 렌더링해서 클라이언트로 보내줌 → 클라이언트에 코드를 저장하지 않음
    - 서버에서 일차적으로 렌더링을 하므로 첫 페이지 로딩이 빠름
    - 친구에게 페이지를 공유할 때 SPA의 경우 원하는 데이터가 전달되지 않는 경우가 많음
        - 브라우저 상단의 타이틀이나, 페이지 내 정보가 공유에 적합하지 않을 때가 있음
- **정적 사이트** (서버가 필요 없는 static website)에 유리함
    - 코드가 프레임워크으로 정해진 경우가 많아 생산성이 좋음(반대로 그 프레임 워크를 쓰지 않을 때는 다시 배워야함...?)
    

서버 사이드 렌더링이므로 모듈을 가져올 때 충돌이 발생하는 경우가 많다. (모듈마다 사용법이 다르다.)

→ plugins 디렉토리에 넣어서 사용해야한다. (해당 모듈에 issue를 확인할 것)

### nuxt.config.js

- html과 비슷한 역할을 한다

Auto import components

- components 내부에 있는 파일만 가능
- 그 외에는 디렉토리 path를 지정해주어야한다 🤔

## 동작 살펴보기

**Dynamic routing**

![Untitled](https://s3-us-west-2.amazonaws.com/secure.notion-static.com/c6fee00c-da82-4753-9853-dc16ee0996d1/Untitled.png)

![Untitled](https://s3-us-west-2.amazonaws.com/secure.notion-static.com/dc2bd92c-b7c7-47ee-aa6d-eafbe85ffdfa/Untitled.png)

- [route.params.id](http://route.params.id) 로 파라미터 접근 가능

- board 안의 create 라우트를 따로 분리할 경우
