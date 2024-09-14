# メモ

風景を場所と紐づけて投稿、閲覧できるアプリケーション
→ 作成理由: 僕が使いたいから

### 最終形
- GoogleMapsAPIを使用して、投稿された場所と投稿内容を視覚的に表示。
- バックエンドはSpringBoot、フロントエンドはReactを使用。
- ユーザーの認証にいつも開発でよく詰まるので、Oauthを使うことを検討(時間と相談)

#### 現状詰まってる場所
- ~~postgresqlとつなげる際になにかミスったようで起動時のデータベース作成がそもそも動いておらず、そのためデータベースにアクセスできない状態。~~(修正済み)
- 雑に作っていったせいで画像をどう扱っていくか決まっていない。 → サーバーに保存して、パスをDBに保存？ Controllerあたりは後で整備
- フロントエンドのデザインが全く決まっていない。 → 一旦templateエンジンを使用してSpringのみで作成しているので機能の実装が終わってから考える。
- SpringSecurity苦手意識あり

#### 実装しないといけないこと
- ユーザー機能
- 現在地と紐づけて投稿になっているがweb上の地図から場所を指定して投稿ができるようにする。
- 画像の扱い
- デザイン

#### 懸念点 
- GoogleMapsAPIのマーカーが確かこの前別のものに刷新されたので前の経験が約に立たない気がするから苦労するかも 参考↓
https://digipress.info/tech/migrate-to-google-maps-api-advanced-marker-element/

# 指摘
wikiかREADMEに最低限以下の情報を記載しておくと良い
- プロジェクトの概要(このリポジトリにはどんな機能があるか)
- 必要なライブラリとバージョン
- 開発環境の構築方法

参考
https://karaage.hatenadiary.jp/entry/2018/01/19/073000#:~:text=%E8%80%83%E3%81%88%E3%81%A6%E3%81%84%E3%81%BE%E3%81%99%E3%80%82-,%E6%9C%80%E5%88%9D%E3%81%AB%E3%82%A2%E3%82%A4%E3%82%AD%E3%83%A3%E3%83%83%E3%83%81%E7%94%BB%E5%83%8F%E3%81%AA%E3%81%A9%E3%82%92%E8%A1%A8%E7%A4%BA,-%23%20%E3%83%AA%E3%83%9D%E3%82%B8
```
# リポジトリ名
このソフトはどんなもので、何ができるのかを書く
合わせて、簡単なデモ（使用例）などスクリーンショットやGIFアニメで表示

## Dependency
使用言語とバージョン、必要なライブラリとそのバージョンを書く

## Setup
セットアップ方法を書く。用意するハードウェアとソフトウェアをセットアップするためのコマンドを記載する

## Usage
使い方。なるべく具体的に書く。サンプルも書く

## License
This software is released under the MIT License, see LICENSE.

## Authors
作者を明示する。特に、他者が作成したコードを利用する場合は、そのコードのライセンスに従った上で、リポジトリのそれぞれのコードのオリジナルの作者が誰か分かるように明示する（私はそれが良いと思い自主的にしています）。

## References
参考にした情報源（サイト・論文）などの情報、リンク
```

