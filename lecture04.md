# <第4回課題>

## VPC (Virtual Private Cloud)
- AWS 内で作成する仮想ネットワークのこと

## 1.VPC 構築
![VPC詳細](images/VPC-lec04.png)

- ### 1-2.VPC リソースマップ
![VPC2](images/VPC2-lec04.png)

- ### 1-3.VPC サブネット
![サブネット1](images/subnet-1-public.png)
![サブネット2](images/subnet-2-private.png)
![サブネット3](images/subnet-3-public.png)
![サブネット4](images/subnet-4-private.png)

<br><br>
## 2.EC2 構築
![EC2詳細](images/EC2-lec04.png)
<br><br>
## 3.RDS 構築
![RDS詳細](images/RDS-lec04.png)
<br><br>

## 4.セキュリティグループ
- ### 4-1. EC2
![EC2-sg](images/EC2-sg.png)
- ### 4-2. RDS-インバウンド
![RDS-sg](images/images/RDS-sg ｲﾝﾊﾞｳﾝﾄﾞ.png)
- ### 4-3. RDS-アウトバウンド
![RDS-sg](images/RDS-sg ｱｳﾄﾊﾞｳﾝﾄﾞ.png)

<br><br>

## 5. EC2からRDSへ接続
- ### 5-1. EC2にSSH接続してから、EC2にMySQLをインストール
 - $ sudo yum install mysql  
 
 - ![MySQLインストール](images/MySQL- install.png)
 
　
- #### 最初、MySQLのインストールが出来ないエラーが発生
　- このエラーについて色々と原因を追及し試した上で、最終的にネットワークACLが原因だと理解し、確認して変更したことで解決する
　
　- ![ネットワークACL変更前](images/ ﾈｯﾄﾜｰｸACL-before.png)
　- ![ネットワークACL変更後](images/ ﾈｯﾄﾜｰｸACL-after.png)
　
- ### 5-2. RDSへの接続
 - $ mysql -u admin -p -h データベースのエンドポイント
 - パスワード入力が求められるので、設定したパスワードを入力する
 
 - ![RDSへの接続](images/EC2-RDS-lec04.png)
