# package

- gem: パッケージ管理
- Rakefile: 定型業務などを記述して実行できるファイル
- bundle: gemパッケージを明示的に示すためのコマンド
- Gemfile: gemパッケージを設定ファイル
- Gemfile.lock: Gemfileに記述されているgemパッケージの依存関係を解決した結果が保存されている


# Railsの思想

- CoC(Convention over Configuration)
- DRY(Don't Repeat Yourself)
- REST(Representational State Transfer)
- 自動テスト

レールに乗ることにより高い生産性を実現ことができるが安全で高速なアプリケーションを開発するのが難しくなるのは事実

どのように開発を進めていくかがエンジニア腕の見せ所

# 主要なファイルやディレクトリ

- .ruby-version: rbenvなどを利用している場合、このファイル内に記載されているバージョンのRubyを利用する
- Gemfile:  このプロジェクトで利用するgemファイルを定義したファイル
- Gemfile.lock: Gemfileの依存関係を解決した結果を保存する
- app/: 主なアプリケーションコードを記述するディレクトリ
- bin/: アプリケーション開発のための実行コマンドを格納しているディレクトリ
- config/: アプリケーションの動作に関する設定ファイルを格納するディレクトリ
- db/: DBに関する設定を格納するディレクトリ
- lib/: Rakeタスクなどアプリケーションから独立したコードを格納するディレクトリ
- public/: 静的コンテンツを配置するディレクトリ
- test/: テストに関するソースコードをまとめるディレクトリ


Model, View, ControllerのMVCアーキテクチャを採用している

railsコマンド
- db:create データベースを作成する
- db:drop データベースを削除する
- db:migrate マイグレーションファイルの内容をテーブル定義をDBに反映させる
- db:seed db/seeds.rbの内容を実行する
- db:setup データベースを作成し、スキーマの読み込みとシードデータの読み込みを行う
- routes URLとControllerを紐づいているルーティング情報を出力する
- runner 任意のスクリプトを実行する
- stats ControllerやModelなどの行数などを集計したデータを表示する



