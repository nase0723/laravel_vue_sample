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
`cd app`

`composer require laravel/ui:3.*`

## vueのベースを作る
`php artisan ui vue`

## 認証追加
`php artisan ui vue --auth`

## フロントエンドパッケージインストール
`npm install`

`npm install vue-loader@^15.9.8 --save-dev --legacy-peer-deps`

## Vue3を使う場合
`npm uninstall vue && npm uninstall vue-loader && npm uninstall vue-template-compiler`
`npm i -save-dev laravel-mix@next vue@next && npm i -D @vue/compiler-sfc && npm i vue-loader`

## Vue Routerインストール
`npm install vue-router@3`

## フロントエンドビルド実行
`npm run dev`
