# JENKINS AUTO BUILD TEST
# JENKINS AUTO BUILD TEST
# JENKINS AUTO BUILD TEST

# README
デプロイテスト用のプロジェクト
rails sで公開 (nxinx/unicornなし)

### 環境変数の設定
```
EC2_MYSQL_SOCKET=/var/lib/mysql/mysql.sock
EC2_MYSQL_PASSWORD='DB接続パスワード'
DB_HOST_NAME='localhost => 適宜変更'
S3_BUCKET_NAME='S3のバケット名'
AWS_ACCESS_KEY_ID='S3接続ユーザのアクセスキー'
AWS_SECRET_ACCESS_KEY='S3接続ユーザのシークレットキー'
```

### clone後
```
$ cd photo_upload_app_for_s3
$ bundle exec rails db:create
$ bundle exec rails db:migrate
$ rails s -b 0.0.0.0
```
