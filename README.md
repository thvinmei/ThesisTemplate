# 学位論文テンプレート

このリポジトリは，修士論文を作成したときに利用したLaTeXファイルを，他の人も利用できるように編集・公開したものです．

各ファイルにはipsumパッケージによるダミーテキストが挿入されています．

# ファイルとディレクトリの構成
## mainファイル(.tex)
mainファイル内には一部のタイトルや著者情報など以外は記入せず，他のファイルをincludeする前提で作成しています．

### 論文本体のmainファイル
- main.tex
### 要旨本体のmainファイル
- sum.tex

## プリアンブルに相当するファイル
読み込むスタイルファイルは以下のstyファイルの中にまとめて書き込むことで，main,sumのどちらでも共通で読み込まれるようになっています．
- libs.sty

また，以下のstyファイル内に作成する文書の書式関係の情報を書き込むことで，main,sum両方で共通した書式が適用されるようになっています．
- format.sty

## 文献情報ファイル(.bib)
Mendeley等の文献管理システムで自動生成されるファイルと，手動入力したファイルを別のファイルとして保管します．
- Ref-Auto.bib
- Ref-Manual.bib

## 本文TeXファイル(.tex)
本文は各章・節毎に分割したtexファイルに入力することを想定しています．

ただし，Summary.texの内容については，main.tex，sum.tex両方から読み込まれるようになっています．

## 画像ディレクトリ
画像等を入れるためのディレクトリとしてFigsディレクトリが作成されています．
ダミー用の画像として，Figs/DUMMY.pngが保存されているので，これを仮の画像として文書作成にしようして構いません．
(このLaTeXテンプレートを使用する場合に限り，DUMMY.pngの利用に制限を設けません)
- Figs/
- Figs/DUMMY.png