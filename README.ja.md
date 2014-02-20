## バイオインフォマティクスのためのスモールツール**宣言**

この **宣言** は、現在の生物学的および生命医学的研究のためのソフトウェアとパイプラインを設計するにあたっての目的、規約、そして推奨されることについて述べるものである。

研究における大規模なデータ取得は次の様な課題をもたらした。すなわち、
(1) 計算における規模の拡大 (2) データ全体の統合 (3) データ操作と可視化である。われわれは、「ボタンを押すだけ」のような解決策へ向かう研究者たちのために、「巨人の方に乗り」、モジュール化され、柔軟でオープンな方法でソフトウェアを構築する重要性に対する視点を研究者コミュニティーが失いつつあると考える。

この **宣言** は、研究所や企業がエンドユーザーを対象とした一枚岩的なソフトウェアを作成しているような現在のバイオインフォマティクスにおける潮流に反対するものである。この **宣言**は、各々の部分が簡単に交換できるような効率的なコンピュータ上の解決法を作るために、モジュール化され連結可能な方法で使えるスモールツールを試してきたUnixコンピュータの伝統に基づく。この宣言はまた、真に「自由ソフトウェアおよびオープンソースソフトウェア（FOSS）」ではないソフトウエアライセンス供与の現在の潮流に反対するものである。たとえ真にFOSSであるライセンスによって作成されたソフトウェアが、学術用途に限るものも含んだオープン性が低いライセンスに最終的に打ち勝つことを歴史が示したとしても、われわれはこのような **宣言** が必要であると考える。

*バイオインフォマティクスのためのスモールツール* は、生物学および生命医学データに携わる研究者、ソフトウェア開発者、統計学者およびシステム管理者より構成される。

*バイオインフォマティクスのためのスモールツール* は、研究プロジェクト間での「車輪の再発明」や、たとえば、シークエンシングパイプラインにおける再現できるような記述された解決策の欠如について憂慮している。

*バイオインフォマティクスのためのスモールツール* は、Unixの伝統の中における小規模な共同作業ツールとソフトウェアによる解決策に関するものである。

*バイオインフォマティクスのためのスモールツール* は、自由ソフトウェアおよびオープンソースソフトウェアを作り、ソフトウェアによる解決策を共有し、結果の再現性と透明性を奨励する。

*バイオインフォマティクスのためのスモールツール* は各々のツールが容易に理解でき、テストでき、交換できるようなモジュール化された解決策の構築を同意する。

*バイオインフォマティクスのためのスモールツール*  はひとつの救済策であり、ビッグデータに適した解決策をひとつに集めこれらのツールを相互作用させる方法を作り出すための先進的な中央での取り組みである。

以下に述べるシンプルな規約が *バイオインフォマティクスのためのスモールツール*  に署名する者すべてに適用される：

* すべての各々のツールは、可能な限り小さいタスクを本当に上手に行うべきである。

* すべての各々のツールは、それらのための公共のソースコードレポジトリに存在する。

* すべてのツールは自由ソフトウェアおよびオープンソースソフトウェア（FOSS）であり、自由ソフトウェア財団 Free Software Foundation (FSF)により承認されたライセンスに基づく。

* ソースコードは、有能な開発者にとって読みやすく理解しやすいものであるべきである。 

* エラー条件と例外は記述されたものであり、明確な方法で扱うことができるべきである。
  
* 可能ならば、ツールは（Unixの）パイプをサポートすべきである。

* 可能ならば、ツールは使いやすいコマンドラインインターフェースを提供すべきである。

＊ツールは名前付き（絶対）ファイルパスのようなシステム依存性を避けるべきである

* すべての各々のツールは少なくともLinuxのためのシンプルなビルド手順とともに入手できなければならない

* ソフトウェアのインストールとデプロイメントのための依存性は外部のパッケージ管理システムを通して扱われる。

以下は推奨されるものである。

* GitHubおよび同等なものをソースコードのホスティングに使用する。

* Travisおよび同等なものを自動化テストに使用する。

* GNUパッケージシステム（GUIX）のためのパッケージ定義を提供する。

* この **宣言** の基準に合致するすべてのツールは、世界中で標準的なバイオインフォマティクスパイプラインの一部になる。

このバイオインフォマティクスのためのスモールツール **宣言** は以下の者によって署名されている。

1. [Pjotr Prins](http://thebird.nl/)
2. [Raoul Bonnal](https://github.com/helios)
3. [Francesco Strozzi](https://github.com/fstrozzi)
4. [Artem Tarasov](https://github.com/lomereiter)

どうぞこの文書をクローンし、コピーし、ブログに載せて下さい。オリジナルは https://github.com/pjotrp/bioinformatics で見つけることができます。

注釈：
現時点ではバイオインフォマティクスはシークエンシングの大当たりで繁栄している。異論のあるところではあるが、現状のソフトウェア工学での取り組みはビッグデータの要求に真に適合するものではないために、バイオインフォマティクスは機器に直面している。それほど昔でないころから、プログラマーはPerl、Python、RあるいはCといった（小さい）ツールに特化して書くことでなんとかしのいできた。今日、バイオインフォマティクスソフトウエア工学は、マルチコアプログラミング、入出力ボトルネック、RAMの制限、そしてわがままなユーザーを扱わなければならない。全体的な課題は、ひとりの孤立した学生が次の大きな全機能含むソフトウェアを書こうするような仕事としては大きすぎるものになってきている。われわれは、生物学、統計学、ソフトウェア開発、そしてシステム管理の背景をもつ研究者をまきこんだ共同作業による取り組みにますます依存するようになっている。これは、


This is
where the **MANIFESTO** kicks in - by encouraging researchers and students to come out
of isolation and write small tools that can be bolted together with other
tools.

Also, there is a lack of good work flow management solutions in bioinformatics
pipelines, a gap that sits somewhere between generic cluster management
software, such as Sun Grid Engine, on the one end, and user oriented work flow
solutions, such as Galaxy, on the other.  This gap has led to sequencing
centres around the world creating their own scripted and often fragile
pipelines, thereby reinventing the wheel and ending with a semi-optimal and
hard to maintain work flow solution. This  **MANIFESTO** calls for a collaborative
effort in changing the way we write software for pipelines and making
such bioinformatics software pipelines simpler, flexible,
'antifragile' and more manageable.

The **MANIFESTO** accentuates command line tools with a clear input/output stream
supporting (Unix) pipes, which make the components of a (sequencing) pipeline.
Also for web based tools and GUI programs, most of above rules and
recommendations are applicable. By making software solutions self contained and
modular they become pluggable and can be easily replaced by a new generation of
tools. Software is software. Software should be easy to change, replace and
improve. The **MANIFESTO** champions that philosophy.

訳注：
@mishimahryk による試訳です。翻訳版は https://github.com/misshie/bioinformatics で見つけることができます。

