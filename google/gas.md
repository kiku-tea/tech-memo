# Google App Scripts
---

## Webページ
### ウェブアプリ作成
1. Googleドライブ -> スクリプト作成
2. ファイル -> New -> Htmlファイル -> ファイル名"index"で作成
3. スクリプト -> myFunctionをdoGetに変更
4. doGet内に以下を記載
  ```
  function doGet(e){
    return HtmlService.createHtmlOutputFromFile('index');
  }
  ```
5. デプロイ -> 実行者自分、アクセス全員 -> 完了

### CSS読み込み
1. ファイル -> New Htmlファイル -> ファイル名"css"で作成
2. ファイル内をすべて削除し、以下を記述
   ```
   <style></style>
   ```
3. index.htmlのheadを以下に変更
   ```
   <head>
   <base target="_top">
   <?!= HtmlService.createHtmlOutputFromFile('css').getContent(); ?>
   </head>
   ```
4. スクリプトファイルのdoGet内を変更
   ```
   function doGet(e){
    return HtmlService.createTemplateFromFile('index').evaluate();
  }
   ```
5. デプロイ

### 