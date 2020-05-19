# Youtube

Yukihiro NAKAJIMAのYoutube([Link](https://www.youtube.com/channel/UCsgvpTZyI4Cgyv5Vv2CbBtA/videos?view_as=subscriber)) で解説したRのコードを掲載します.

## 前提
`tidyverse`パッケージはインストール済みであることを前提とします.
まだの方は, Cosoleで次のコードを実行してください.

```
install.packages("tidyverse")  # 初回のみ
```

## 公開するもの1

授業の回数に応じたR notebookを公開します．
各自こちらのコードを参考に演習を進めてください．

## 公開するもの2

各回の授業スライドで用いた図表のソースコードを提示します.
図表の意味をソースコードから理解したい方は確認してください.
なお, 図表は基本的にtikz及びggplot2を用いて作成しています.

## フォルダ・ファイルのコピーの仕方

次のコードをRのconsole上で実行することでこのレポジトリを各自のフォルダにコピーできます．

初回は次のようにコードを実行します．
```
install.packages("git2r")  # 初回のみ
library(git2r) # 利用時は毎回
url <- "https://github.com/N-Yukihiro/Statistics_YNU2020_exercise.git"
clone(url = url,
      local_path = "exercise") # 初回のみ
```

このgithubのレポジトリが更新された場合は，次のようにコードを実行してフォルダの内容を更新し, 各自R notebookをコピーしてください．

```
library(git2r) # 利用時は毎回
config(user.name="Unkown", user.email="test@example.com") # 初回のみ．各自の名前やメールアドレスに変更．
setwd("exercise")
git2r::pull()
```

## フォルダ構成

フォルダの構成としては, 各回の講義ごとにフォルダを作成します.
各講義回の下層に`exercise`と`figure`のフォルダがあります(各回でR演習がなければ`exercise`フォルダがなく, 図表を用いなければ`figure`フォルダはありません).

`exercise`は項目別にノートブックとしてまとまっており, `figure`はスライド内の図表番号と拡張子の前の数字が一致するようにしています.

なにかわからないことがあれば担当者まで気軽にご連絡ください.
