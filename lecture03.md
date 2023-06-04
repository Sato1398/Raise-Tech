# lecture03
## APサーバー
- APサーバーの名前・・・Puma
- バージョン・・・Ver 5.6.5
- APサーバーを終了させた場合、Oopsと表示され、アクセスできない。起動するとアクセス可能。
## DBサーバー
- DBサーバーの名前・・・MySQL
- バージョン・・・Ver 8.0.33
- DBサーバーを終了させた場合、エラーが出てアクセスできない。
- sudo service mysqld start:MySQLサーバーを起動
- sudo service mysqld stop:MySQLサーバーを停止
- sudo service mysqld restart:MySQLサーバーを再起動
- sudo service mysqld status:MySQLサーバーの状態確認
## Railsの構成管理ツール
- bundler:gemのバージョンやgemの依存関係を管理するツール
## 今回の課題から学んだこと
### RVMを使ったRubyのインストール
- RVM:Ruby Version Manager
- rvm help:使用可能なコマンドの表示
- rvm get master:最新のRVM開発バージョンをインストール
- rvm install:Rubyのインストール
### Ruby on Railsによる Webアプリケーションの起動
- Puma:Railsに標準で付随しているAPサーバー
- rails s:APサーバーの起動
- Ctrl+C:APサーバーの停止(Windows)
### Linuxコマンド
- ls:ディレクトリ情報の一覧表示
- cd:ディレクトリ移動、カレントディレクトリ変更
- mkdir:フォルダ作成
- touch:ファイルの作成
- cp:ファイルのコピー
- which:コマンドの保存先の調査
- sudo:スーパーユーザーの権限でコマンドを実行する(ユーザーを切り替えなくてもいい)
### npm
- Node Package Managerの略
- Node.jsのパッケージ管理ツール
### Yarn
- 比較的新しく、2016年にFacebookが開発したnode.jsのパッケージ管理ツール
- npmと互換性がある
- npmに比べ実行速度が高速
- package.jsonが使用できる
### ファイル・ディレクトリの権限(パーミッション)の確認方法と変更方法
- ls -l:ファイルの詳細情報を確認
- パーミッションは左から所有者、グループ、その他のユーザー
- パーミッションの対応表
| アクセス権 | 数値 | 説明 |
| :-----: | :-: | :-------------- |
| --- | 0 | 読み込み書き込み不可 |
| --x | 1 | 実行のみ |
| -w- | 2 | 書き込みのみ |
| -wx | 3 | 書き込み実行のみ |
| r-- | 4 | 読み込みのみ |
| r-x | 5 | 読み込み実行のみ |
| rw- | 6 | 読み込み書き込みのみ |
| rwx | 7 | 読み込み書き込み実行ができる |
- chmod:パーミッションの変更
## その他の単語
### socket(ソケット)
- 物理的な接続端子
- ソフトウェア間で通信する仕組み、ネットワークとの接続口
### config(コンフィグ)
- 設定