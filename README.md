# t3s3_test
T3S3のテストケースの自動化を行う。

テストケースは下記チケットの資料を参照してください
https://www.tool.sony.biz/common-jira/browse/RETRO-1543

## ディレクトリ構成
```bash
t3s3_test
│  run_all.bat              # script配下にあるスクリプトを一括実行するスクリプト
│
├─log                       # 各テストのログを格納
│  ├─xxxxxx                 # テスト仕様書 - 「xxxxxx」テストのログを格納
│      ：
│
└─script                    # 各テストのスクリプトを格納
    │  setting.txt          # 共通環境変数設定ファイル
    │  TERATERM.INI         # Teraterm環境設定ファイル
    │
    ├─xxxxxx                # テスト仕様書 - 「xxxxxx」テストのスクリプトを格納
        ：
```

## 環境準備
- Tera Termをインストールする。  
- 任意のフォルダに本リポジトリのフォルダを格納する。  
- setting.txt は環境に合わせて修正する。  
- TERATERM.INI の接続先ポート(ComPort)等は環境に合わせて修正する。  
- maxpwrtestを実行する場合は以下を実施する。  
  * script/maxpwrtestにあるnginxフォルダをhttpサーバにするホストの実行ユーザのホームディレクトリに配置する。  
  * nginxフォルダ内のREADME.txtを参照してnginxコンテナイメージをロードする。  
  * 実行ユーザがdockerグループに所属していない場合は以下コマンドで所属させる。(sudoなしでdockerコマンドが実行できること。)  
      sudo gpasswd -a <ユーザ名> docker
