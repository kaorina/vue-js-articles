## このリポジトリについて
### Ruby on RailsとVue.jsで構築した説明用のサンプルアプリです。
内容はブログ記事の管理アプリです。
ベースの実装はRuby on RailsのScaffoldコマンドで作成し、その後Vue.jsで実装しています。

[説明記事はこちら](http://qiita.com/kaorina/items/ea365be58da73d23b54b)

## 開発環境について
以下環境にて動作確認済みです。
* Mac OS X EI Capitan (10.11.6)
* Ruby 2.3.0
* Vue.js 2.4.2

### その他環境
* Ruby on Rails 5.0.5 (4.2.0でも動作確認済)
* MySQL2

### config/database.ymlについて
git cloneしたらターミナル上で

```
cp config/database.yml.sample config/database.yml
```
としてからconfig/database.ymlをご自身の環境に応じて編集してください。

### .ruby-versionについて
Rubyのバージョンを変更する場合は.ruby-versionファイルを編集してください。

### データベースの作成、migrationの実行について
下記コマンドで行ってください。

```
./bin/rake db:create
./bin/rake db:migrate
```
