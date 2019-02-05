# sublime-settings-sync
Sublimeの同期をGitで行う．  
[sublimetext公式](https://packagecontrol.io/docs/syncing)  
[参考にした日本語ブログ](https://www.kimurak.net/wordpress/sublimetext/1786/)  

# Usage
クローン先

  - Linux   ~/.config/sublime-text-3/Packages/User
  - Windows    ~\AppData\Roaming\Sublime Text 3\Packages

# 動作確認環境
  - windows10
  - ubuntu18.04

# 大体の設定方針
  - tabよりSpace
  - markdown
  - python
    - pyenv使用
  - エディタでbuildはしない

# 環境依存的設定
## 共通
  - 

## ubuntu
  - SublimeMozcInput  
  [http://yasuyuky.github.io/SublimeMozcInput/](http://yasuyuky.github.io/SublimeMozcInput/)
  - 

## windows10
  - IMESupprt
    - 入れてもズレることがある．ディスプレイの解像度設定のせい．

# 依存まとめ
## ubuntu
###  apt install
	sudo apt install emacs-mozc # SublimeMozcInput用
### gitとかから
  [Ricty Diminished Discord](https://www.rs.tus.ac.jp/yyusa/ricty_diminished.html)