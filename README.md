# vim-ignmod
読み書き権限をガン無視してVimを起動させるためのやつ

なお、スーパーユーザーでの使用を想定

## インストール
1. `vim-ignmod`を環境変数PATHに書いてあるディレクトリのどこか(`~/.local/bin/`など)にダウンロードして、実行権限を与える
2. シェルの設定ファイルに以下のような行を追加する
```.bashrc
alias vim="vim-ignmod \"${@}\""
```

```config.fish
alias vim="vim-ignmod \"$argv\""
```

## 使い方
いつも通りにVimを起動すればOK
