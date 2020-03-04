# pc-env

## local

chocolateryを使って開発環境を整備する。

### chocolateryのinstall

https://chocolatey.org/install#installing-chocolatey

### アプリケーションのinstall

`choco install -y git nodejs yarn golang python vscode googleChrome teraterm`

### install済みアプリケーションの一覧

`choco list -lo`

### git init

```bash
git config --global user.email "you@example.com"
git config --global user.name "Your Name"
```

## VSCodeの設定

VSCodeの拡張機能`Setting Sync`を用いて管理する。
https://gist.github.com/utadachiren/0fca9f69a9f04eeaecce6218351a5bf0

## wslの設定

[ここ](https://simplestar-tech.hatenablog.com/entry/2019/10/14/101551)を参考にubuntuをinstall

### nodebrew

[ここ](https://www.kimoton.com/entry/20190215/1550166179)を参考にnodeをinstall。npm, yarnも勝手に入る。

### docker

[公式Doc](https://docs.docker.com/v17.06/engine/installation/linux/docker-ce/ubuntu/#install-using-the-convenience-script)を参考にinstall。
`sudo service docker run`の際に、wslを管理者権限で実行している必要があるので注意。