# pc-env

chocolateryを使って開発環境を整備する。

## chocolateryのinstall

https://chocolatey.org/install#installing-chocolatey

## アプリケーションのinstall

`choco install -y git nodejs yarn golang python vscode googleChrome`

## install済みアプリケーションの一覧

`choco list -lo`

## git init

```bash
git config --global user.email "you@example.com"
git config --global user.name "Your Name"
```

## wslの設定

* [ここ](https://simplestar-tech.hatenablog.com/entry/2019/10/14/101551)を参考にubuntuをinstall

### VSCodeのターミナルをbashにする

**※ここはvscodeの設定リポジトリに移動予定**

* settings.jsonに以下を追加
    
    `"terminal.integrated.shell.windows": "C:/Windows/Sysnative/bash.exe"`
