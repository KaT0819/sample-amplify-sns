# sample-amplify-sns


## setup
```
# create react app
npx create-react-app boyaki

cd boyaki

# amplify init
amplify init

# ライブラリ追加
npm install --save aws-amplify@3.4.3 @aws-amplify/ui-react@1.2.1
```

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


## 認証追加
```
amplify add auth

Do you want to use the default authentication and security configuration? Default configuration
 Warning: you will not be able to edit these selections.     
 How do you want users to be able to sign in? Username       
 Do you want to configure advanced settings? No, I am done.
```





## amplify command
```
# リソース一覧
amplify status

# デプロイ
amplify push

```