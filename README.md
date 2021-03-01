# pc-env

## local

chocolateryを使って開発環境を整備する。

### スクリプトの実行ポリシーの変更

スクリプトの実行が無効化される場合があるので、実行ポリシーを変更しておく。

```
# 管理者権限でPowershellを開き、以下を実施
PowerShell Set-ExecutionPolicy RemoteSigned
```

### chocolateryのinstall

https://chocolatey.org/install#installing-chocolatey

### アプリケーションのinstall

* `choco install -y git nodejs yarn golang python vscode googleChrome teraterm docker-desktop`

### install済みアプリケーションの一覧

`choco list -lo`

### git init

```bash
git config --global user.email "you@example.com"
git config --global user.name "Your Name"
```

### clasp - GASのgit管理

1. claspのinstall

    ```
    npm i @google/clasp -g
    ```

2. GAS API を 設定

    [ここ](https://script.google.com/home/usersettings)にアクセスしてAPIをONに

3. clasp login

    ```
    clasp login
    ```

## VSCodeの設定

VSCodeの拡張機能`Setting Sync`を用いて管理する。
https://code.visualstudio.com/docs/editor/settings-sync

## wslの設定

[ここ](https://simplestar-tech.hatenablog.com/entry/2019/10/14/101551)を参考にubuntuをinstall

### git init

```bash
git config --global user.email "you@example.com"
git config --global user.name "Your Name"
```

### nodebrew

[ここ](https://www.kimoton.com/entry/20190215/1550166179)を参考にnodeをinstall。npm, yarnも勝手に入る。

### docker

docker desktopがinstallされている前提で、docker desktopのdaemonを利用します。

1. [公式Doc](https://docs.docker.com/v17.06/engine/installation/linux/docker-ce/ubuntu/#install-using-the-convenience-script)を参考にinstall。
2. `docker.exe version`でversion確認
