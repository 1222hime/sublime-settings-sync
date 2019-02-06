# sublime-settings-sync
Sublimeの同期をGitで行う．  
[sublimetext公式](https://packagecontrol.io/docs/syncing)  
[参考にした日本語ブログ](https://www.kimurak.net/wordpress/sublimetext/1786/)  
ノートパソコンが高DPI設定のせいで日本語入力がずれるので，それ対策をしてみた．

# Usage
クローン先

  - Linux   `~/.config/sublime-text-3/Packages/User`
  - Windows   ` ~\AppData\Roaming\Sublime Text 3\Packages`

# 動作確認環境
  - windows10 (ノートパソコン)
  - ubuntu18.04

# 大体の設定方針
  - tabよりSpace
  - markdown
  - python
    - pyenv使用
  - エディタでbuildはしない

# 環境依存的設定
## 共通
### 本文のfont  
  等幅のNotoフォントにしたけど，行間が広すぎるのでSettingで行間を詰めた．  
  [Noto Sans CJK JP](https://www.google.com/get/noto/)は手動でインストール．
  
  Rictyはなんかよくわからんエラーメッセージ吐いていたので首にした．  
  他のフォントに比べて明らかに小さいし．  
  つよう人いたら理由教えてほしいね．
### sideberとかのフォントサイズ 
  themeを入れたときにFontサイズが好みじゃないので変更した．  
  `選んだテーマ.sublime-theme`の中身でフォントサイズを変えられる．  
  今は `Adaptive.sublime-theme`

## ubuntu
### SublimeMozcInput  
  日本語入力がいい感じになる．Tabで変換候補が出る．  
  [http://yasuyuky.github.io/SublimeMozcInput/](http://yasuyuky.github.io/SublimeMozcInput/)

## windows10
### IMESupprt  
 日本語入力のズレを治すパッケージだが，入れてもズレることがある．  
 ディスプレイ設定で，`拡大縮小とレイアウト`が100%じゃなかったらおこる．  
 microsoftへの怒りを抑えてどっちかの設定をすれば良い．

1. `拡大縮小とレイアウト`を100%にする．  
    1. 全体的にフォントサイズが小さくなっちゃうので["Meiryo UIもだいっきらい"](https://tatsu-syo.github.io/index.html)でフォントサイズを大きくした (ついでに好きなフォントに変えちゃった)．  
    1. chrome等，別のアプリもその都度フォントサイズの設定を変更する．
    1. 昔はフォントサイズだけ大きくできたらしいので，またできるようになるのを願う．
1. sublimetextのDPI設定を変更する
    1. 検索で`sublimetext.exe`がある場所を探す．
    1. 右クリックでプロパティを開き，互換性のタブにある高DPIの設定を開く
    1. プログラムDPIにチェックを入る．`次の場合，メインディスプレイに設定されているDPIを使用する`はどっちを選んでもいい．
    1. 高DPIスケールの上書きにチェックを入れ，`アプリケーション`または`アプリケーション(拡張)`を選択する．
    1. Sublimetextの起動が遅くなる．


# 依存まとめ
## ubuntu
###  apt install
	sudo apt install emacs-mozc # SublimeMozcInput用
### gitとかから
  [Noto Sans CJK JP](https://www.google.com/get/noto/)  

以下首にしたやつ  
  [Ricty Diminished Discord](https://www.rs.tus.ac.jp/yyusa/ricty_diminished.html)