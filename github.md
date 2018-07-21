# github勉強会20180722@IAMAS

## 今日のゴール

* gitがなんとなく分かる
* githubがなんとなく分かる
* 自分のWebサイトができる

## git（ギット）とは

ああ〜ファイルを編集前の状態に戻したい

***gitならできるよ***

### バージョン管理

日記＋タイムマシン

## コミットする

* `git init` でリポジトリを作成
* `git add ファイル名` でコミットしたいファイルを指定する
* `git commit -m "コミットメッセージ"` でコミットする

```
$ git init
$ vi hoge.md
$ git add hoge.md
$ git commit -m "initial commit"
```

確認

```
$ git log
```

## リポジトリ

ファイルやディレクトリの状態を記録する場所

### ローカルリポジトリ

さっき作った

### リモートリポジトリ

専用のサーバに配置

***github使う***

### ローカル/リモートの反映

* `git push` でローカルの変更をリモートに反映
* `git pull` でリモートの最新をローカルに反映

## github（ギットハブ）とは

ソースコード管理サービス

他にもなんかいろいろできる

## アカウント作成

[https://github.com/](https://github.com/)

## リモートリポジトリ作成

* `New Repository` をクリック
* `Repository name` は一旦 `[アカウント名].github.io` （本来はなんでもよい）
* `Create Repository` をクリック

## 自分のWebサイトを作る

* `Settings` > `GitHub Pages` > `Theme Chooser`
* 適当なテーマを選んでWeb上でコミット
* `https://[アカウント名].github.io/` を確認

```
$ git clone https://github.com/[アカウント名]/[リポジトリ名]
$ vi index.md
$ git add hoge.md
$ git commit -m "Fix index.md"
$ git push origin master
```

もう一度 `https://[アカウント名].github.io/` を確認して変更が反映されていれば成功
