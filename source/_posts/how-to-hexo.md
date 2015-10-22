title: 本サイト用のHexo利用方法
date: 2015-10-22 18:12:00
tags: Hexo
---

## 初期インストール
```console
npm i hexo-cli -g
git clone -b src https://github.com/exmatrix/exmatrix.github.io.git blog
cd blog
npm i
```

## 新しい記事の作成
```console
hexo new "directory-name"
```

## 記事のチェック
```console
hexo server
```

## アップロード
```console
hexo deploy -g
```

_config.ymlの`deploy:`の部分は
```yaml
deploy:
  type: git
  repo: https://exmatrix@github.com/exmatrix/exmatrix.github.io.git
  branch: master
```
のようにすることで、ユーザー名を省略できます。