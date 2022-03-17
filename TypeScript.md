# TypeScript 

## typescript handbook
[URL(영문)](https://www.typescriptlang.org/docs/handbook/typescript-from-scratch.html)

## typescript 설치
[참고 URL](https://medium.com/@rnrjsah789/vscode-%EC%97%90%EC%84%9C-typescript-%ED%99%98%EA%B2%BD-%EC%84%A4%EC%A0%95%ED%95%98%EA%B8%B0-e40c9cbc2dd5)

```
npm i -D typescript // devDependency로 설치
npm i -g typescript // global로 설치
```

## ESLint 설치 및 설정 (**<span style="color: red">TSLint는 더이상 사용하지 않음.</span>**)

```
npm install -D eslint @typescript-eslint/eslint-plugin @typescript-eslint/parser
```
* eslint 세부 설정  
.eslintrc.json 파일에 작성

* .eslintrc.json rules  
https://github.com/typescript-eslint/typescript-eslint/tree/main/packages/eslint-plugin#supported-rules

* no-inferrable-types  
```
  "rules": {
    "@typescript-eslint/no-inferrable-types": "off"
  }
```
* eslint 예외 처리 방법  ([eslint ignore](https://worker-k.tistory.com/entry/%EC%97%84%EA%B2%A9%ED%95%9C-eslint-ignore-%ED%95%98%EB%8A%94-%EC%97%AC%EB%9F%AC%EA%B0%80%EC%A7%80-%EB%B0%A9%EB%B2%95-eslintignore))  
.eslintIgnore 파일에 예외 처리할 경로 작성

## ESLint와 Prettier 함께 사용하기
* 코드 분석기인 ESLint와 formatter인 Prettier를 함께 사용하기  
https://pravusid.kr/javascript/2019/03/10/eslint-prettier.html

---