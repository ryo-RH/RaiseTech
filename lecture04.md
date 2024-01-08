# <第4回課題>

## VPC (Virtual Private Cloud)
  - AWS 内で作成する仮想ネットワークのこと
<br>

## VPC 構築
![VPC構築](./VPC.1-img.png)


<br>

## EC2 構築
![EC2構築](./EC2.1-img.png)

## EC2 セキュリティーグループ
![EC2](./EC2.2-img.png)

<br>
<br>


## RDS 構築
![RDS構築](./RDS.1-img.png)


<br>
<br>

## EC2からRDSへ接続
![EC2からRDSへの接続](./EC2-RDSへの接続.img.png)


<br>
<br>
<br>

     
### * EC2にSSH接続してから、EC2にMySQLをインストール
- $ sudo yum install mysql

### * RDSへの接続
- $ mysql -u admin -p -h データベースのエンドポイント
- パスワード入力が求められるので、設定したパスワードを入力する



