# cakephp.2016

本リポジトリは選択授業「Learning Web Development Framework」に関する情報展開用です

## 評価方法

- 出席 50%
- 演習 50%

## 演習


### 8/1

1. 「初心者のためのCakePHP3 プログラミング入門」を進める
1. 上記の成果物をadd/commit
1. リモートリポジトリへpush

### 7/25

1. 各自の環境にcakephpをインストール
1. cakephpをgitのローカルリポジトリとして管理(add/commit)
1. ローカルリポジトリをGitHubのリモートリポジトリとしてpush  
リポジトリ名: cakephp.2016

### 7/11

1. Virtualbox&Vagrantにより各自の環境設定

## 開発環境の設定

### 1. Virtualboxのインストール

#### ubuntu

1. システムのアップデート  
$ sudo apt update
1. システムのアップグレード  
$ sudo apt upgrade
1. VirtualBoxのインストール  
$ sudo apt install virtualbox

#### mac

1. VirtualBoxの入手&インストール  
<a href="https://www.virtualbox.org/wiki/Downloads" target="_blank">ここから入手</a>

### 2. Vagrantのインストール

1. Vagrantの入手&インストール  
<a href="https://www.vagrantup.com/downloads.html" target="_blank">ここから入手</a>  

### 3. 仮想環境の設定

1. vagrant box の追加  
$ vagrant box add cakephp package.box
1. 仮想環境を保存するディレクトリを作成し移動  
$ mkdir ~/cakephp  
$ cd ~/cakephp
1. Vagrantfile作成  
$ vagrant init cakephp
1. Vagrantfilel編集
$ vi Vagrantfile  
で、ファイルを開き、以下のコメントアウトを外す  
\# config.vm.network "forwarded_port", guest: 80, host: 8080
1. 仮想環境起動  
$ vagrant up
1. ssh接続  
$ vagrant ssh


## 授業で使用するサイトのリンク

- <a href="http://book.cakephp.org/3.0/ja/installation.html" target="_blank">CakePHP 3.xのインストール手順</a>
- <a href="http://libro.tuyano.com/index2?id=4536003" target="_blank">初心者のためのCakePHP3 プログラミング入門</a>

## 関連リンク

- <a href="http://book.cakephp.org/3.0/ja/orm.html" target="_blank">データベースアクセス & ORM</a>
- <a href="http://jmatsuzaki.com/archives/16505" target="_blank">CakePHP3.xでのAuthコンポーネントの使い方</a>
- <a href="https://www.phpmyadmin.net/downloads/" target="_blank">phpMyAdminダウンロード</a>