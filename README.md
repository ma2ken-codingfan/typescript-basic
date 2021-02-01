# 日本一わかりやすい TypeScript 入門

## url

[日本一わかりやすい TypeScript 入門](https://www.youtube.com/watch?v=qSHlXcSces8&list=PLX8Rsrpnn3IW0REXnTWQp79mxCvHkIrad&index=2)

[github](https://github.com/deatiger/ts-basic-demo)

## install

```bash
npm init

npm install -g typescript
npm install --save-dev typescript ts-loader webpack webpack-cli webpack-dev-server

tsc --init

// develop
npm run start

// production
npm run build
```

## 2. ESLint と Prettier の CI 環境を構築

```bash
npm install --save-dev eslint eslint-config-prettier prettier @typescript-eslint/parser @typescript-eslint/eslint-plugin husky lint-staged
```

### 2-2. husky がもし動かなかったら

.git/hooks が正常に作成されていない可能性アリ これで確認する
ls -la .git/hooks/ls -la .git/hooks/

.sample しかなかったら NG
NG の場合はインストールし直す npm uninstall huksy
npm install --save-dev husky
もう一度 hooks を確認
ls -la .git/hooks/ls -la .git/hooks/
