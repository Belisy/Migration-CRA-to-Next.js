# CRA를 Next.js로 마이그레이션 하기

1. yarn create react-app cra-to-next-migration
2. yarn remove react-scripts
3. yarn add next
4. "scripts" 수정
5. .gitignore 수정 (# dependencies > .next 추가)
6. 이미지파일은 public으로 옮기기
7. 루트경로>pages생성>\_document.js생성>  
   public>index.html의 head부분을 \_document.js파일에 옮기기  
   (cf) \<title>태그는 \_app.js파일로 옮기기)
8. pages>\_app.js생성>global.css파일 import
9. styles폴더생성>global.css생성>App.css와 index.css파일 복붙, App.css,index.css삭제
10. pages>index.js생성 > src>App.js복붙, App.js삭제
11. src>index.js 삭제
12. yarn dev
13. yarn build
14. yarn start
