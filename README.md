# Project 환경 설정

## ES Lint, Prettier 설정

1. npm i -D eslint
2. npm i -D --save-exact prettier
   > --save-exact 는 정확한 버전을 설치하게 guide 해준다
3. npm i -D eslint-config-prettier eslint-plugin-prettier
   > eslint-config-prettier : eslint 와 prettier 과 겹치는 포맷을 비활성화
   > eslint-plugin-prettier : eslint 에 prettier 포매팅 룰을 설정해준다
4. npx eslint --init
   > .eslintrc 파일이 생기며 초기화 해준다
5. .eslintrc.json(혹은 js) 파일에 eslit-plugin-prettier extention을 추가해준다

```js
  extends: ['eslint:recommended', 'plugin:react/recommended', 'prettier']

6. .eslintignore 파일을 만들어 준다
   > 제외할 파일, 폴더를 설정한다(node_module, webpack.config, dist 등)
7. .prettierrc.json 파일을 생성한다
```
