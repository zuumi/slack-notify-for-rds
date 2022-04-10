## 目的

停止されたRDSは7日以上経過すると自動で起動してしまうため，自動で停止（起動→停止）する設定を追加した
その際に，RDSの状況をSlackに投稿するため，このLambdaを用意した．

## Serverless Framework で SNS + Lambdaを作成

環境は MacOS/Linux

```
$ curl -o- -L https://slss.io/install | bash
```

```
$ sls create --template aws-python3
```

## デプロイ

```
$sls deploy -v
```

## 参考記事

https://www.serverless.com/framework/docs/getting-started/
https://www.serverless.com/framework/docs/providers/aws/cli-reference/create/
https://www.serverless.com/framework/docs/providers/aws/cli-reference/deploy/
https://qiita.com/ikasama/items/b1ccbc9cde80c137405b
