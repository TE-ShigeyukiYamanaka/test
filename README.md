# ws_discovery_ddcl_test
T3 WS-Dのテストケースの自動化を行う。

## ディレクトリ構成
```bash
ws_discovery_ddcl_test
│  run_all.bat              # script配下にあるスクリプトを一括実行するスクリプト
│
├─log
│  ├─prm                    # パラメータテスト(初期化、デバイス検索)の実行ログ等を格納
│  ├─seq                    # シーケンステストの実行ログ等を格納
│  └─setup                  # パラメータテスト(デバイスセットアップ)の実行ログ等を格納
│
└─script
    │  setting.txt          # 共通環境変数設定ファイル
    │  t3_connect.ttl       # WS-D自動起動マクロ
    │  t3_memory_check.vbs  # T3メモリ使用量取得スクリプト
    │
    ├─prm                   # パラメータテスト(初期化、デバイス検索)のスクリプトを格納
    ├─seq                   # シーケンステストのスクリプトを格納
    └─setup                 # パラメータテスト(デバイスセットアップ)のスクリプトを格納
```

## 環境準備
- Tera Termをインストールする。  
- DDCLサンプルアプリケーション（DDCL_UserSample.exe等）を任意のフォルダに格納する。  
- DDCLサンプルアプリケーションを配置したフォルダに本リポジトリのフォルダを格納する。  
- setting.txt は環境に合わせて修正する。  
- t3_connect.ttl の接続先ポート等は環境に合わせて修正する。  

```bash
任意のディレクトリ
│  DDCL.dll
│  DDCL.lib
│  DDCL_UserSample.exe
│  run_all.bat
│
├─log
│  ├─prm
│  ├─seq
│  └─setup
│
└─script
    │  setting.txt
    │  t3_connect.ttl
    │  t3_memory_check.vbs
    │
    ├─prm
    │   prm_xxx_xxxxxxxxx.bat
    ├─seq
    │   seq_xxx_xxxxxxxxx.bat
    └─setup
        prm_xxx_xxxxxxxxx.bat
```
