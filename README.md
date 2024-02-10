# [MultiPie チュートリアル](https://cmt-mu.github.io/MultiPieTutorial/)

- はじめに

    群論操作および対称性適合多極子基底生成ライブラリ[MultiPie](https://github.com/CMT-MU/MultiPie)に関するチュートリアルです。
    求めたい情報を具体的に掲げて、それに答える形で操作方法を例示しています。

    3D描画ツール[QtDraw](https://github.com/CMT-MU/QtDraw)では、本ライブラリを使用しています。

    QtDrawのチュートリアルは、[こちら](https://cmt-mu.github.io/QtDrawTutorial/)。

- 引用に関して

    科学研究でQtDrawやMultiPieを用いた場合には、以下を引用していただければ幸いです。
  > Hiroaki Kusunose, Rikuto Oiwa, and Satoru Hayami, Symmetry-adapted modeling for molecules and crystals, Phys. Rev. B <b>107</b>, 195118 (2023).<br>
  > DOI: [https://doi.org/10.1103/PhysRevB.107.195118](https://doi.org/10.1103/PhysRevB.107.195118)

- その他の事項

  - 執筆ガイドライン

    * Markdownのセルで、数式の記述には`$$`, `$$ $$` 環境を用いる。
    * 文献は、ノートブックの末尾のmarkdownセルに、リストで掲載。
    * 文献は`references.bib`に追加可。

- GitHub Pagesの環境設定

    ```bash
    $ pip3 install jupyter-book ghp-import jupytext
    $ git switch --orphan gh-pages
    $ git rm -rf *
    $ touch .nojekyll
    ```

- 内容の更新
  - ローカルのmainブランチで行う。
  - src内に記事ファイルを作成。
  - _toc.ymlを適切に更新。
  - GitHubの更新 (gh-pagesへcommit, push)
    ```bash
    make upload
    ```

- トラブル・シューティング
  * https://github.com/executablebooks/jupyter-book/issues/1541
