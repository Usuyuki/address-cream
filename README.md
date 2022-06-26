<!-- @format -->

# address-cream

🍦 アドレスバーで遊ぶための JS ライブラリ(アドレスバーとアイスクリームをもじった)

### 単調に増やしていく

```
addressCream.constant("寿司食べたいかも", 0.2);
```

### 単調に増やしていく+パーティクル

```
addressCream.constant("寿司食べたい", 0.2, "✨", "🍣", 0.5);
```

### 単調に増やして、単調に戻す

```
addressCream.goBack("寿司食べたいかも？なんだ、気のせいか。", 0.2,0.1);
```

### 電光掲示板みたいにする

```
addressCream.goBack("途中の停車駅は、品川、名古屋、京都、新大阪、新神戸、岡山、小倉、博多です。",0.3,7);
```

![address-cream-demo](https://user-images.githubusercontent.com/63891531/175813979-61cbadf1-f00c-439f-a362-7f3ca9686098.gif)

# テストの方法

ブラウザ上のやつを使う(location.系が cli でできないため)

runner.html を開く → 結果が出る。以上

ブラウザ無しで行ける系なら yarn test。

## テストを作れていないので代替手段

src/index.js の末尾から 1 つめのコメントアウトを解除、2 つめをコメントアウト
check/index.js で試す

# 参考記事

[オリジナルの JavaScript ライブラリを公開しよう](https://zenn.dev/yusuke99/books/fcd96342f5cb1b468799)

[TypeScript + Mocha/Chai 非同期テストコードメモ](https://qiita.com/olisheo/items/99ba5dfad317e9bd332b)

[Mocha と Chai でなんでもテスト ～ブラウザ用 JavaScript 編～](https://note.kiriukun.com/entry/testing-with-mocha-and-chai---browser-javascript)
