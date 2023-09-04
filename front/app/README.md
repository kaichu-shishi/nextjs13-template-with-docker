# Next.js13（App Router安定版）をDockerで環境構築したもの

## クイックスタート
- パッケージマネージャー
  - このプロジェクトはパッケージマネージャーとして「yarn」を使用しています。「yarn」をインストールしておいてください
- リポジトリのクローン
  - `$ git clone https://github.com/kaichu-shishi/nextjs-app-docker.git`
  - または、手動でzipファイルをダウンロードして解凍する
- ディレクトリの移動
  - `$ cd ./nextjs-app-docker`
  - ※手動でダウンロードした場合は`$ cd ./nextjs-app-docker-main`
- イメージビルド
  - `$ docker-compose build`
- パッケージインストール(初回または、新たにパッケージが導入された時のみ)
  - `$ docker-compose run --rm front yarn install --frozen-lockfile`
- コンテナ起動
  - `$ docker-compose up -d`
- ブラウザで表示
  - `http://localhost:3000`にアクセスしてNext.jsの画面が表示されたら成功です！

## 環境詳細
- Next.js13.4.19（with TypeScript、TailwindCSS）
- ESLintとPrettierを使用