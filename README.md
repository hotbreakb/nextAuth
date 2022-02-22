## 실행 영상
https://user-images.githubusercontent.com/64337152/155147960-62d8f150-3610-4a46-ae16-f60b5eb9f78f.mov


## 네이버

- Redirect URI: http://localhost:3000/api/auth/callback/naver

## 카카오

- clientId: REST API 키
- clientSecret: 내 애플리케이션 -> 왼쪽 사이드바에서 보안 -> 발급 후 사용
- Redirect URI: http://localhost:3000/api/auth/callback/kakao
  - 설정: 내 애플리케이션 -> 왼쪽 사이드바에서 제품 설정 -> 카카오 로그인

### error🔥 Redirect URI 확인하는 법

- 에러난 페이지에서 `new URL(document.referrer).searchParams.get("redirect_uri")`를 콘솔창에 입력
- 출처: [네이버](https://help.naver.com/support/contents/contents.help?serviceNo=17063&categoryNo=17795&from=alias)

### error🔥 The default export is not a React Component in page: "/"

- arrow function을 function()으로 바꾸면 된다.
- 출처: [stackoverflow](https://stackoverflow.com/questions/59873698/the-default-export-is-not-a-react-component-in-page-nextjs)

### error🔥 next-auth node version downgrade

- `$ nvm install 버전`
- `$ nvm use 버전`

### 참고자료

- [NextAuth.js](https://next-auth.js.org/getting-started/example)
- [한국어 설명](https://blog.toycrane.xyz/7분만에-next-auth-알아보기-d4432ff97158)
