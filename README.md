# ws_discovery_ddcl_test
T3 WS-Dのテストケースの自動化を行う。

## ディレクトリ構成
```bash
ws_discovery_ddcl_test
├─log
│  ├─prm          # パラメータテストの実行ログ等を格納
│  └─seq          # シーケンステストの実行ログ等を格納
│
└─script
   ├─prm          # パラメータテストのスクリプトを格納
   └─seq          # シーケンステストのスクリプトを格納
```

## 環境準備
サンプルアプリケーション（DDCL_UserSample.exe等）を任意のフォルダに格納します。  
サンプルアプリケーションを配置したフォルダに本リポジトリのフォルダを格納します。

```bash
任意のディレクトリ
│  DDCL.dll
│  DDCL.lib
│  DDCL_UserSample.exe
│
├─log
│  ├─prm
│  └─seq
│
└─script
    ├─prm
    │   prm_xxx_xxxxxxxxx.bat
    └─seq
        seq_xxx_xxxxxxxxx.bat
```
