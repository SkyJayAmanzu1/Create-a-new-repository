# LIFF 最小スターター（申込履歴 / 相談履歴）

## 目的
まずは LIFF を触るための最小構成です。

- LINE 内で開く
- `liff.init()` を実行する
- LINEプロフィールを取得する
- Azure Functions の履歴 API を呼び出す

## ファイル
- `index.html`
- `README.md`

## 先に置き換える場所
### 1. LIFF ID
```js
const LIFF_ID = "YOUR_LIFF_ID";
```

### 2. Azure Functions のベースURL
```js
const API_BASE_URL = "YOUR_FUNCTION_BASE_URL";
```

例:
```js
const API_BASE_URL = "https://func-line-kintone-dev-01.azurewebsites.net";
```

## 想定API
### 申込履歴
`/api/liff/application-history?lineUserId=...`

### 相談履歴
`/api/liff/consult-history?lineUserId=...`

## 最初の確認
1. LIFF URL を LINE に送る
2. LINE 内で開く
3. プロフィールが表示される
4. API 未実装ならエラー表示でもOK
