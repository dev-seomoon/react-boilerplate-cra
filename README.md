# react-boilerplate-cra

CRA(Create-React-App)를 사용해 생성한 리액트 프로젝트의 보일러 플레이트입니다.  

CRA에서 기본적으로 주어지는 컴포넌트와 스타일을 제거해 실행 시 빈 페이지가 뜨도록 했고,  
테스팅 패키지들과 테스팅 파일들을 제거했습니다.  
주석과 로고, favicon 등의 파일도 모두 삭제했습니다.  

eslint 설정이 필요한 경우 다음 파일을 프로젝트 루트 디렉터리에 추가하면 됩니다. 

.eslintrc.json 
```json
{
  "extends": ["react-app", "plugin:prettier/recommended"]
}
```

사용하는 에디터에서 eslint, prettier를 적용한 적이 없는 경우 추가 설정이 필요합니다.  
VSCode의 경우 마켓플레이스에서 prettier, eslint 플러그인을 설치하고  
settings.json을 다음과 같이 설정하면 됩니다.  
setting 메뉴에서 다음 항목들을 찾아서 직접 설정해줘도 됩니다.  

```json
"editor.formatOnSave": true,
"[javascript]": {
"editor.formatOnSave": false
},
"eslint.autoFixOnSave": true,
"eslint.alwaysShowStatus": true,
"prettier.disableLanguages": ["js"],
"files.autoSave": "onFocusChange"
```

당연히 node_modules은 포함되어 있지 않으므로,  
클론 후 `yarn` (또는 `npm install`) 명령어 실행이 필요합니다.  
