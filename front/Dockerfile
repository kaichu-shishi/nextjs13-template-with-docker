FROM node:18-alpine
WORKDIR /app

# パッケージインストールのためのコマンド追加
COPY ./front/app/package.json ./front/app/yarn.lock ./
RUN yarn install --frozen-lockfile
# 全ファイルをコピー
COPY ./front/app/ ./

# この場合後述のCMD ["yarn", "dev"]のみが適用されて他のコマンドは無視される
CMD [ "yarn", "build" ]
CMD ["yarn", "start"]
CMD ["yarn", "dev"]