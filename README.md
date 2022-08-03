## Dockerデーモンの起動
`sudo service docker start`

## コンテナを立ち上げる
`UID_GID="$(id -u):$(id -g)" docker-compose up -d --build`

## コンテナに入る
`docker-compose exec app bash`

## Laravelプロジェクト作成
`composer create-project laravel/laravel=8.* app --prefer-dist`
.envのDBをdockerコンテナに合わせる

## laravel/uiをインストール
`composer require laravel/ui:3.*`

## vueのベースを作る
`php artisan ui vue`

## 認証追加
`php artisan ui vue --auth`

## フロントエンドパッケージインストール
`npm install`

## Vue3を使う場合
`npm uninstall vue && npm uninstall vue-loader && npm uninstall vue-template-compiler`
`npm i -save-dev laravel-mix@next vue@next && npm i -D @vue/compiler-sfc && npm i vue-loader`

## Vue Routerインストール
`npm install --save vue-router`

## フロントエンドビルド実行
`npm run dev`