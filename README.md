<!-- @format -->

# address-cream

ð¦ ã¢ãã¬ã¹ãã¼ã«æå­åãæµãã©ã¤ãã©ãªã  
ã¢ãã¬ã¹ãã¼(address bar)ã£ã¦ã¢ã¤ã¹ãã¼ã£ã½ãååã ãªã£ã¦æããããããã¢ãã¬ã¹ãã¼ã¨ã¢ã¤ã¹ã¯ãªã¼ã ãæ··ããaddresss-creamã«ãªãã¾ããã  
ã¯ãªã¼ã ã®ããã«ã¢ãã¬ã¹ãå½©ãã¾ãã

https://www.npmjs.com/package/address-cream

# Documentation

### åèª¿ã«å¢ããã¦ãã

```
addressCream.constant('å¯¿å¸é£ã¹ãããã', 0.2);
```
![address-cream-constant](https://user-images.githubusercontent.com/63891531/175817844-fd0369f4-4ecf-40df-8449-4a1f1ff32f81.gif)


### åèª¿ã«å¢ããã¦ãã+ãã¼ãã£ã¯ã«

```
addressCream.constant('å¯¿å¸é£ã¹ãã', 0.2, 'â¨', 'ð£', 0.5);
```
![address-cream-constant-with-particle](https://user-images.githubusercontent.com/63891531/175817847-ffc69371-c3d0-4381-93c6-a6fe22ae832c.gif)

### åèª¿ã«å¢ããã¦ãåèª¿ã«æ»ã

```
addressCream.goBack('å¯¿å¸é£ã¹ããããâ¦â¦ãªãã ãæ°ã®ãããã', 0.2, 0.1);
```
![address-cream-go-back](https://user-images.githubusercontent.com/63891531/175817851-880927c2-e7d4-4cf0-b4fc-a80d7163e139.gif)

### é»åæ²ç¤ºæ¿ã¿ããã«ãã

```
addressCream.flow('éä¸­ã®åè»é§ã¯ãåå·ãåå¤å±ãäº¬é½ãæ°å¤§éªãæ°ç¥æ¸ãå²¡å±±ãå°åãåå¤ã§ãã', 0.3, 7);
```
![address-cream-flow](https://user-images.githubusercontent.com/63891531/175817858-edcf0156-751b-446e-a809-66053439a936.gif)


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
  <head>
    <meta charset="UTF-8" />
    <script src="https://cdn.jsdelivr.net/npm/address-cream"></script>
    <!-- omit -->
  </head>
  <body>
    <!-- omit -->
    <script>
      addressCream.constant("æ¢é¨æãã¡ãã£ãï¼", 0.2);
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
    addressCream.constant('å¯¿å¸é£ã¹ãã', 0.2);
  });
//omit
```



# ãã¹ãã®æ¹æ³(ã¡ããã¨ãã¹ãæ¸ãã¦ã¾ããï¼ï¼ï¼ï¼)

location.ç³»ã cli ã§ã§ããªãããããã©ã¦ã¶ã©ã¤ã¯ãªãã¹ã  
runner.html ã«ãã¹ãæ¸ããããããã©ã¦ã¶ã§éãã¨mochaã®assersionãåãã

ãã©ã¦ã¶ç¡ãã§è¡ããç³»ãªã
```
yarn test
```
ãä½¿ããããç¾ç¶ä½¿ãã¦ããªãâ¦â¦

## ãã¹ããä½ãã¦ããªãã®ã§ä»£æ¿ææ®µ

src/index.js ã®æ«å°¾ãã 2ãã®ã³ã¡ã³ãã¢ã¦ããè§£é¤ã
check/index.js ã§ç´ã«å®è¡ãã¦è©¦ãã

# åèè¨äº

[ãªãªã¸ãã«ã® JavaScript ã©ã¤ãã©ãªãå¬éããã](https://zenn.dev/yusuke99/books/fcd96342f5cb1b468799)

[TypeScript + Mocha/Chai éåæãã¹ãã³ã¼ãã¡ã¢](https://qiita.com/olisheo/items/99ba5dfad317e9bd332b)

[Mocha ã¨ Chai ã§ãªãã§ããã¹ã ï½ãã©ã¦ã¶ç¨ JavaScript ç·¨ï½](https://note.kiriukun.com/entry/testing-with-mocha-and-chai---browser-javascript)
