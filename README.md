# Youtube

Yukihiro NAKAJIMAのYoutube([Link](https://www.youtube.com/channel/UCsgvpTZyI4Cgyv5Vv2CbBtA/videos?view_as=subscriber)) で解説したRのコードを掲載します.

## 前提
`tidyverse`パッケージはインストール済みであることを前提とします.
まだの方は, Cosoleで次のコードを実行してください.

```
install.packages("tidyverse")  # 初回のみ
```

## 公開するもの

授業の回数に応じたR notebookを公開します．
各自こちらのコードを参考に演習を進めてください．

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

動画の公開年月に合わせたフォルダ構成になっています.
適宜動画に沿ったnotebookを御覧ください.

誤りなどを見つけた際は, Googleのアンケートフォームからご指摘ください.
(https://docs.google.com/forms/d/e/1FAIpQLSdfqhUQ2V91kXtS08raQjUr62Xyddkj4Vpd6TcOfAFzQ6HMyQ/viewform?usp=sf_link)
