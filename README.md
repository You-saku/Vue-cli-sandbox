# Vue-cli-sandbox
リポジトリの使い方

```
# リポジトリのクローン
git clone git@github.com:You-saku/Vue-cli-sandbox.git<
or
git clone https://github.com/You-saku/Vue-cli-sandbox.git

# コンテナ起動
cd Vue-cli-sandbox
docker-compose up -d
docker-compose exec vue_app sh

# Vueのプロジェクト作成方法
vue create {プロジェクト名}
＊色々聞かれます(自分は「Vue3」と「Yarn」を選択しています)

# Vueプロジェクトの起動
cd {プロジェクト名}
yarn serve
localhost:3000を開く
```

このリポジトリをクローンしてコピーすればたくさんプロジェクトを作れます。<br>
dockerなので環境は汚れませんし、nodeのバージョンも指定してるので再現性はあります。