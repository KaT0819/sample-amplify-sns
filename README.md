# sample-amplify-sns


## setup
```
# create react app
npx create-react-app boyaki

cd boyaki

# amplify init
amplify init
※ 設定はdefalut


# ライブラリ追加
npm install --save aws-amplify@3.4.3 @aws-amplify/ui-react@1.2.1
```


## 認証追加
```
amplify add auth
```

## API追加
```
amplify add api
```



## エラー
amplify add auth
において下記エラーが発生
```
./node_modules/idb/build/esm/index.js
Module parse failed: Unexpected token (78:4)
You may need an appropriate loader to handle this file type.
| }
| replaceTraps((oldTraps) => ({
|     ...oldTraps,
|     get: (target, prop, receiver) => getMethod(target, prop) || oldTraps.get(target, prop, receiver),
|     has: (target, prop) => !!getMethod(target, prop) || oldTraps.has(target, prop),
```

下記にバージョンを変更することで解消

"react-scripts": "^1.1.5"　⇒　"^4.0.1"
```
npm install
npm start
```




## amplify command
```
# リソース一覧
amplify status

# デプロイ
amplify push

# API モック
amplify mock api

```



## 参考情報
```
# 初期化
amplify init

※ 設定はdefalut
Project information
| Name: boyaki
| Environment: dev
| Default editor: Visual Studio Code
| App type: javascript
| Javascript framework: react
| Source Directory Path: src
| Distribution Directory Path: build
| Build Command: npm.cmd run-script build
| Start Command: npm.cmd run-script start


# 認証追加
amplify add auth

Do you want to use the default authentication and security configuration? Default configuration
 Warning: you will not be able to edit these selections.     
 How do you want users to be able to sign in? Username       
 Do you want to configure advanced settings? No, I am done.


# API追加
? Please select from one of the below mentioned services: GraphQL
? Provide API name: BoyakiGql
? Choose the default authorization type for the API Amazon Cognito User Pool     
Use a Cognito user pool configured as a part of this project.
? Do you want to configure advanced settings for the GraphQL API No, I am done.
? Do you have an annotated GraphQL schema? No
? Choose a schema template: Single object with fields (e.g., “Todo” with ID, name, description)
