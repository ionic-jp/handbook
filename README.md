# Ionic Frameworkでつくる モバイルアプリ開発入門
書籍[「Ionicで作る モバイルアプリ制作入門〈Web/iPhone/Android対応〉](http://amzn.to/2mstNnh)」のサポートページです。著者と[Ionic Japan User Group](https://t.co/K9slM8tvi8)にて運営を行っております。

## チュートリアル
本書のチュートリアルは、以下のレポジトリでステップ別に公開しています。なぜか動かない時などにご利用下さい。
- [チュートリアル「タスクリストアプリをつくってみよう」](https://github.com/Ionic-jp/ionic-tutorial)
- [チュートリアル「WordPressを表示するアプリをつくろう」](https://github.com/Ionic-jp/wp-tutorial)
- [チュートリアル「コードリファクタリング」](https://github.com/Ionic-jp/rf-tutorial)
- [チュートリアル「スマホアプリの機能をつけよう」](https://github.com/Ionic-jp/native-tutorial)

## 本書での誤字・誤植
誤字・誤植についてご案内いたします。「間違った記述もしくはチュートリアルを進めることができないもの」は *致命的な誤字誤植* 、 そうでないものを *その他の誤字誤植* として案内しております。

### 致命的な誤字誤植
- 現在ありません

### その他の誤字誤植
CHAPTER05で誤字誤植がございます。大変申し訳ございません。なお、作業行には影響ありませんので、チュートリアルは問題なく進めていただくことができます。

#### P110 中部 SAMPLE CODE `src/pages/home/home.ts`
`constructor` で呼び出しているモジュール名が間違っている。

```
constructor(
    public http: Http,  =>  public http: HttpClient,
```


#### P119 下部 SAMPLE CODE `src/pages/home/home.ts`
`import` の呼び出し順が間違えている。

```
  import { IonicPage, NavController, LoadingController, Platform } from 'ionic-angular'; => 下
- import { HttpClient } from '@angular/common/http'; => 上
```


#### P122 下部 SAMPLE CODE `src/pages/home/home.ts`
`HttpClient` の削除忘れ / `Platform` の `import` 忘れ

```
import { Component } from '@angular/core';
import { HttpClient } from '@angular/common/http'; => 削除
import { IonicPage, NavController, LoadingController, Platform } from 'ionic-angular'; => Platformの追加
```

#### P123 中部 SAMPLE CODE `src/pages/article/article.ts`
`HttpClient` の削除忘れ

```
import { Component } from '@angular/core';
import { HttpClient } from '@angular/common/http'; => 削除
```
