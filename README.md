# react_docker

DockerでReactの開発環境をつくるためのリポジトリ

## 1. Docker install

[公式より](https://matsuand.github.io/docs.docker.jp.onthefly/get-docker/)

## 2. コンテナ起動

```bash
cd react_docker
mkdir server
docker-compose up -d --build  
docker-compose exec web /bin/sh 
```

webのコンテナから

```bash
yarn create react-app my-app（my-appアプリの名前）
cd my-app
yarn start
```

## 3.スタートページの確認

http://localhost:3000/ 