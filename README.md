<!-- @format -->

# address-cream

🍦 アドレスバーで遊ぶための JS ライブラリ(アドレスバーとアイスクリームをもじった)

https://www.npmjs.com/package/address-cream

# Getting Started
## Installation
```
npm i address-cream
```
or
```
yarn add address-cream
```
or
```
<script src="https://cdn.jsdelivr.net/npm/address-cream"></script>
```

## Usage

### Vanila JS
```
<!DOCTYPE html>
<html lang="ja">
<!-- omit -->
<script src="https://cdn.jsdelivr.net/npm/address-cream"></script>
<!-- omit -->
</head>
<body>
<!-- omit -->
    <script>
      addressCream.constant('寿司食べたい', 0.2);
    </script>
<!-- omit -->
</body>
</html>
```

### Next.js
```
import addressCream from 'address-cream';
//omit
 useEffect(() => {
    addressCream.constant('寿司食べたい', 0.2);
  });
//omit
```


# Documentation

### 単調に増やしていく

```
addressCream.constant('寿司食べたいかも', 0.2);
```
![address-cream-constant](https://user-images.githubusercontent.com/63891531/175817844-fd0369f4-4ecf-40df-8449-4a1f1ff32f81.gif)


### 単調に増やしていく+パーティクル

```
addressCream.constant('寿司食べたい', 0.2, '✨', '🍣', 0.5);
```
![address-cream-constant-with-particle](https://user-images.githubusercontent.com/63891531/175817847-ffc69371-c3d0-4381-93c6-a6fe22ae832c.gif)

### 単調に増やして、単調に戻す

```
addressCream.goBack('寿司食べたいかも……なんだ、気のせいか。', 0.2, 0.1);
```
![address-cream-go-back](https://user-images.githubusercontent.com/63891531/175817851-880927c2-e7d4-4cf0-b4fc-a80d7163e139.gif)

### 電光掲示板みたいにする

```
addressCream.flow('途中の停車駅は、品川、名古屋、京都、新大阪、新神戸、岡山、小倉、博多です。', 0.3, 7);
```
![address-cream-flow](https://user-images.githubusercontent.com/63891531/175817858-edcf0156-751b-446e-a809-66053439a936.gif)


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
