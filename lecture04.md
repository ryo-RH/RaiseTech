# <第4回課題>

## VPC (Virtual Private Cloud)
- AWS 内で作成する仮想ネットワークのこと

## VPC 構築
![lecture04-1]
<br>
<br>
## EC2 構築
![lecture04-2]
<br>
<br>
## RDS 構築
![lecture04-3]
<br>
<br>
## EC2からRDSへ接続
![leture04-4]
<br>
### EC2にSSH接続してから、EC2にMySQLをインストール
- $ sudo yum install mysql

### RDSへの接続
- $ mysql -u admin -p -h データベースのエンドポイント
- パスワード入力が求められるので、設定したパスワードを入力する



