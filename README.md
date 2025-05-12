# mkdocs-dev
mkdocsを試す

## 公式サイト
https://squidfunk.github.io/mkdocs-material/

## ローカル実行
devcontainerを使ってローカルで実行する

## 記事作成
```bash
mkdocs new .
```

## ローカル確認
```bash
mkdocs serve
```

[http://127.0.0.1:8000/](http://127.0.0.1:8000/)にアクセス

portを指定したい場合は以下を参考
```bash
mkdocs serve --dev-addr=127.0.0.1:8080
```

## サイトの公開について
Github Pagesを使って公開することができる
公式：https://squidfunk.github.io/mkdocs-material/publishing-your-site/#publishing-your-site

- Github Actionsを使って自動でデプロイすることができる
    - 実行した際に権限でエラーが出る場合は、リポジトリのSettings > Actions > General > Workflow permissionsがRead and Write になっているか確認する。

- Github Pagesの設定
    - 公式：https://docs.github.com/en/pages/getting-started-with-github-pages/configuring-a-publishing-source-for-your-github-pages-site
    - Settings > Pages > Sourceをgh-pages branchにする
    - Github PagesのURL
        - https://<username>.github.io/<repository-name>/
