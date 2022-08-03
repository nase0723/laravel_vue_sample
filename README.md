## Dockerデーモンの起動
`sudo service docker start`

## コンテナを立ち上げる
`UID_GID="$(id -u):$(id -g)" docker-compose up -d --build`

## コンテナに入る
`docker-compose exec app bash`

## Laravelプロジェクト作成
`composer create-project laravel/laravel=8.* app --prefer-dist`

## laravel/uiをインストール
`composer require laravel/ui:3.*`

## 認証追加
`php artisan ui vue --auth`

<!-- ## npm install
`curl -o- https://raw.githubusercontent.com/nvm-sh/nvm/v0.39.1/install.sh | bash`
`source ~/.bashrc`
`nvm install --lts`

## vue.js install
`npm install vue@next vue-loader@next @vue/compiler-sfc` -->

## コンパイル
`npm install`
`npm run dev`