# Node.js_webpack-demo
WPJさんの「サンプルで学ぶwebpack 2入門」の記事を参考に作成

## このサンプル制作時の環境
* Windows10 Pro、64bit、32GB

## 事前に用意するもの
* Node.js（本サンプル制作時はv8.4.0）

## 開発手順（win:cmd、mac:tarminal）
1. npm install （package.jsonにあるライブラリがインストールされる）
1. npm start （src内ファイル監視状態で起動。終了は ctrl+C 。）
1. npm run build （public/js/bundle.js が minify で出力される）

## npm installでインストールされるライブラリ
* babel-core
* babel-loader
* babel-preset-es2015
* css-loader
* file-loader
* node-sass
* sass-loader
* style-loader
* url-loader
* webpack

## gulpで実行されること
* src ＞ public/js へbundle.jsファイル出力（src内のapp.jsを中心に他ファイル情報をまとめて一つにする）

## 参考リンク
* [サンプルで学ぶwebpack 2入門：Web開発を超効率化する必須ツールの使い方 - WPJ](https://www.webprofessional.jp/beginners-guide-to-webpack-2-and-module-bundling/)

## 知っておくと便利なnpmコマンド一覧
* `npm root -g` … グローバルのルート（node_modules）を調べる
* `npm root` … プロジェクトのルート（node_modules）を調べる
* `npm ls -g --depth=0` … グローバルにインストールされているパッケージを確認
* `npm ls --depth=0` … プロジェクトにインストールされているパッケージを確認
* `npm init -y` … package.jsonをプロジェクトに生成（オプション「-y」が全てyes回答のショートカット）
* `npm install xxxxx --save` … プロジェクトにパッケージをインストールし、情報を「package.json」に書き込む（dependencies）
* `npm i xxxxx -s` … 上記のショートカットキーバージョン
* `npm install xxxxx --save-dev` … プロジェクトにパッケージをインストールし、情報を「package.json」に書き込む（devDependencies-開発用）
* `npm i xxxxx -D` … 上記のショートカットキーバージョン
* `npm -v` … npmのバージョンを表示
* `npm run` … package.json - scriptに記載した一覧が見れる
* `npm show` … package.jsonを表示
* `npm remove -g xxxxx` … グローバルのパッケージをアンインストール
* `npm remove xxxxx` … プロジェクトのパッケージをアンインストール
