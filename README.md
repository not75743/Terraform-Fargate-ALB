# これはなに？
terraformでECS(Fargate)+ALBの構成を作るリポジトリです。

# 何が出来る？
以下の構成が作れます。  
![](./pictures/fargate-alb.svg)

terraform実行後にALBのパブリックDNSが出力されるため、そこからアクセス可能です。

# 注意
セキュリティは考慮されていません。  
ALBのセキュリティグループのinboundは`0.0.0.0/0`と開放されています。