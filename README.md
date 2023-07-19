# ws_discovery_ddcl_test
---
## 概要
T3 WS-Dのテストケースの自動化を行う。

## ディレクトリ構成
- script　：　スクリプトを格納
- log　：　スクリプトの実行結果を格納

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
    └─seq
            seq_01_initialize_normal.bat

```
