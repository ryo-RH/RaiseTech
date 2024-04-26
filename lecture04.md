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
- ### 4-2. RDS-sgインバウンド
![RDS-sgインバウンド](images/RDS-sgインバウンド.png)

- ### 4-3. RDS-sgアウトバウンド
![RDS-sgアウトバウンド](images/RDS-sgアウトバウンド.png)

<br><br>


## 5. EC2からRDSへ接続
- ### 5-1. EC2にSSH接続してから、EC2にMySQLをインストール
 - $ sudo yum install mysql  
 
- ![MySQL-インストール](images/MySQL-install.png)
 
　
- #### 最初、MySQLのインストールが出来ないエラーが発生
　- このエラーについて色々と原因を追及し試した上で、最終的にネットワークACLが原因だと理解し、確認して変更したことで解決する
　
 <br><br>
 
　- ネットワークACL修正前 ![ネットワークACL変更前](images/ネットワークACL-before.png)
　
 <br><br>
 - ネットワークACL修正後 ![ネットワークACL変更後](images/ネットワークACL-after.png)
　
- ### 5-2. RDSへの接続
 - $ mysql -u admin -p -h データベースのエンドポイント
 - パスワード入力が求められるので、設定したパスワードを入力する
 
 - ![RDSへの接続](images/EC2-RDS-lec04.png)