## バイオインフォマティクスのための小規模ツール**宣言**

この **宣言** は、現在の生物学的および生命医学的研究のためのソフトウェアとパイプラインを設計するにあたっての目的、規約、そして推奨されることについて述べるものである。

研究における大規模なデータ取得は次の様な課題をもたらした。すなわち、
(1) 計算における規模の拡大 (2) データ全体の統合 (3) データ操作と可視化である。われわれは、「ボタンを押すだけ」のような解決策へ向かう研究者たちのために、「巨人の方に乗り」、モジュール化され、柔軟でオープンな方法でソフトウェアを構築する重要性に対する視点を研究者コミュニティーが失いつつあると考える。

この **宣言** は、研究所や企業がエンドユーザーを対象とした一枚岩的なソフトウェアを作成しているような現在のバイオインフォマティクスにおける潮流に反対するものである。この **宣言**は、各々の部分が簡単に交換できるような効率的なコンピュータ上の解決法を作るために、モジュール化され連結可能な方法で使える小規模ツールを試してきたUnixコンピュータの伝統に基づく。この宣言はまた、真に「自由ソフトウェアおよびオープンソースソフトウェア（FOSS）」ではないソフトウエアライセンス供与の現在の潮流に反対するものである。たとえ真にFOSSであるライセンスによって作成されたソフトウェアが、学術用途に限るものも含んだオープン性が低いライセンスに最終的に打ち勝つことを歴史が示したとしても、われわれはこのような **宣言** が必要であると考える。

*バイオインフォマティクスのための小規模ツール* は、生物学および生命医学データに携わる研究者、ソフトウェア開発者、統計学者およびシステム管理者より構成される。

*バイオインフォマティクスのための小規模ツール* は、研究プロジェクト間での「車輪の再発明」や、たとえば、シークエンシングパイプラインにおける繰り返すことのできるような記述された解決策の欠如について憂慮している。

*バイオインフォマティクスのための小規模ツール* は、Unixの伝統の中における小規模な共同作業ツールとソフトウェアによる解決策に関するものである。

*バイオインフォマティクスのための小規模ツール* は、creates free and open source software, shares
software solutions, and encourages transparency and reproducibility of results.

*Small tools for bioinformatics* allows the building of modular solutions where
individual tools can easily be understood, tested and replaced.

*Small tools for bioinformatics* is a rescue plan and forward looking central
effort to bring together solutions suitable for big data analysis and create
ways of having these tools interact with each other.

The following simple rules apply to anyone signing up to *Small tools for
bioinformatics*

* Every single tool should do the smallest possible task really well

* Every single tool lives in its own public source code repository

* All tools are free and open source software (FOSS) and come with a license
    approved by the Free Software Foundation (FSF).

* Source code should be easy to read and understand for a competent software
    developer
  
* Error conditions and exceptions should be descriptive and handled in 
    a clear way

* When possible tools should support (Unix) pipes

* When possible tools provide a useful command line interface 

* Tools should avoid system dependencies, such as named (absolute) file paths

* Every single tool comes with a simple build protocol, at least for Linux

* Software installation and deployment dependencies are handled through 
    external package management systems

The following are recommendations 

* Use github or similar for hosting source code

* Use travis or similar for automatic testing

* Provide a package definition for the GNU package system (GUIX)

* All tools that match the criteria of the **MANIFESTO** will be part of
    standard bioinformatics pipelines across the world

This **MANIFESTO** *Small tools for bioinformatics* is signed by 

1. [Pjotr Prins](http://thebird.nl/)
2. [Raoul Bonnal](https://github.com/helios)
3. [Francesco Strozzi](https://github.com/fstrozzi)
4. [Artem Tarasov](https://github.com/lomereiter)

Please clone, copy, BLOG this document. The original can be found at 
https://github.com/pjotrp/bioinformatics

NOTES

At this point bioinformatics is thriving because of the sequencing bonanza.
Arguably, bioinformatics is in a crisis because existing software engineering
efforts are not really matching the requirements of big data. Not so long ago,
programmers got by writing specialised (small) tools in Perl, Python, R or C.
Today, bioinformatics software engineering has to deal multi-core programming,
with IO bottlenecks, RAM constraints, and demanding users. The overall
challenge has become too large a job for the isolated student trying to
write the next great all-inclusive software solution. We are increasingly
depending on collaborative efforts involving researchers with a background in
biology, statistics, software development and system administration. This is
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

