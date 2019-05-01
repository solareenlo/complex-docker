# complex-docker [![Build Status](https://travis-ci.org/solareenlo/complex-docker.svg?branch=master)](https://travis-ci.org/solareenlo/complex-docker)
**Live Demo**: http://multidocker-env.25ccpzrsad.us-east-1.elasticbeanstalk.com

## 本番環境でのフローチャート
![本番フローチャート](https://github.com/solareenlo/complex-docker/blob/master/images/flowchart_production.png)

## 対応付け
|Docker|->|AWS|
|---|---|---|
|Dockerコンテナ(Nginx, Express, React)|->|AWS VPC|
|Redis|->|AWS Memcached|
|Postgres|->|AWS RDB|
|Docker-compose|->|VPCセキュリティグループ|


## 開発環境でのフローチャート
![開発フローチャート](https://github.com/solareenlo/complex-docker/blob/master/images/flowchart.png)

## ローカルで開発バージョンを動かしたときのスクショ
![スクショ](https://github.com/solareenlo/complex-docker/blob/master/images/Screenshot.png)

## Usage
### ローカル環境での動かし方
```bash
git clone git@github.com:solareenlo/complex-docker.git
cd complex-docker
git checkout local
docker-compose up
```
そして, 任意のブラウザで`localhost:3050`を開く.
