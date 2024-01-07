# <第4回課題>

## VPC (Virtual Private Cloud)
  - AWS 内で作成する仮想ネットワークのこと
<br>

## VPC 構築
![VPC構築](./vpc.1-img/png)

![VPC  CIDER 　　　　エビデンス](https://github.com/ryo-RH/RaiseTech/assets/147240434/4f079983-d483-4537-a643-00d4dc4c347d)


<br>

## EC2 構築
![lecture04-2]![EC2 構築エビデンス](https://github.com/ryo-RH/RaiseTech/assets/147240434/10d32b32-abbf-443c-bab3-da7b736b6987)
### EC2 セキュリティーグループ
![EC2 セキュリティグループ](https://github.com/ryo-RH/RaiseTech/assets/147240434/db477f18-13da-455d-b4dd-82e1ca4970de)


<br>
<br>


## RDS 構築
![lecture04-3]![RDS 構築 エビデンス](https://github.com/ryo-RH/RaiseTech/assets/147240434/d3a541a0-977f-4e1d-9cef-ad1e0aca577f)


<br>
<br>

## EC2からRDSへ接続
![leture04-4]![EC2 から RDS への　接続 エビデンス](https://github.com/ryo-RH/RaiseTech/assets/147240434/3e8e5548-a85d-467c-a7ca-ff192ee2e29d)


<br>
<br>

     
### EC2にSSH接続してから、EC2にMySQLをインストール
- $ sudo yum install mysql

### RDSへの接続
- $ mysql -u admin -p -h データベースのエンドポイント
- パスワード入力が求められるので、設定したパスワードを入力する



