# 環境セットアップ手順
jupyterは自前のを利用する想定

* 必要なライブラリをインストール
```
$ pip install -r requirements.txt
```
psycopg2がなければ別にいれてください。

* DB用ボリュームを作成
```
$ docker volume create dss-postgres-data
```

* docker-composeでDBを起動
```
$ docker-compose up -d
```

* jupyterを起動
```
$ jupyter lab
```

