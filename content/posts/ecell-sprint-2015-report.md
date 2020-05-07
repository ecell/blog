+++
date = 2015-09-21T08:00:00Z
lastmod = 2020-05-07T08:00:00Z
author = "Kozo Nishida"
title = "E-Cell Sprint 2015を日吉で行いました"
subtitle = ""
feature = ""
+++

今年度のE-Cell Sprintを8月29日~9月1日の4日間、慶應義塾大学日吉キャンパスで開催しました。
E-Cell SprintはSystems biology全般に係わるprojectを募り、hackathon形式で開発を行う合宿です。
今年度は下記のような成果が得られました。E-Cell Sprintは来年も開催する予定ですのでご興味を持たれた方はsprint@e-cell.orgまでご連絡ください。

{{< figure src="image/ecell-sprint-2015-report/imgp0422_upload.jpg" >}}

{{< figure src="image/ecell-sprint-2015-report/img_1387.jpg" >}}

|||||
| -- | -- | -- | -- |
| 加藤 傑 | 京都大学 | Cellular Potts Modelの簡易実装 | Cellular Potts Modelを２次元平面上で簡易的にC++を使って実装しました。 |
| 西田 圭吾 | 大阪大学 | 一分子専用フィルタの機械学習による獲得 | 低毒性一分子感度一細胞蛍光イメージングを行うことを目的として、低S/N像から高S/N像を再現するため、機械学習技術の一つである畳み込みニューラルネットワークを細胞イメージングに合うように実装した。 |
| 渡部匡己 | 理研 | 凝集モデルの構築とそのPALMイメージング | 現在、PALMイメージングを使って、細胞性粘菌のcAR1受容体の極性や局在を計る課題に取り組んでいる。PALMを使った一分子計測には、一分子の蛍光特性や選択効率を数値化するためのカリブレーションを欠かすことはできない。今回のE-CELL Sprintでは、詳細な一分子のカリブレーションを行うための蛍光分子の凝集モデルを構築して、そのPALMイメージングのシミュレーションを実装をした。 |
| 熊上 尚樹，神野祥子，瀧口真央，田中雄一郎，脇田舞子（50音順） | 慶應義塾大学 | HuVEC modelのVisual BasicからMATLABへの書き換え | HuVEC modelについて、細胞膜上のイオンチャネルや交換体タンパク・収縮機構をそれぞれ分担し、MATLABへの書き換え作業を行った。 |
| Satya Arjunan | RIKEN QBiC | Particle simulation model of multiple membrane binding states of PTEN | I have successfully implemented full particle simulation model of PTEN which recapitulates its multiple membrane binding states. The model however is unable to reproduce the initial membrane binding probabilities of different states since we assume PTEN is homogeneously distributed in the cytosol. The difference in membrane binding probabilities could be caused by clustering and rebinding effects of cytosolic PTEN. |
| 海津一成 | 理研QBiC | 遺伝子リストと流束から常微分方程式モデルを自動生成するGarudaガジェットの作成 | Garudaプラットフォームは生物学に関わる様々なデータベース、解析ツールや実験機器間をデータを介して自由に行き来できるようにするソフト ウェア間のネットワーキングを目的としたプラットフォームである。今回、大腸菌を対象として遺伝子リストと静的なFBAによって得られた流束データから動 的な常微分方程式モデルを自動生成するガジェットを作成した。これによりユーザは目的とするFBAモデルに対して時間応答を予測できるモデルを用意に作成し、様々なシミュレータに受け渡すことができるようになった。 |
| 新稲亮 | 京都大学 | 物体表面を運動する粒子の拡散運動シミュレーション | 三次元構造体の表面に存在する物体の運動のシミュレーションに必要な機能を備えたポリゴンライブラリの作成。 |
| 深澤風土 | 慶應義塾大学 | 深層学習器の分解再構築 | マルチモーダル学習器のデータの作成と、その下処理を行なった。 |
| 渡邉 麗 | 慶應義塾大学 | 深層学習器の分解再構築 | DEAPを利用した遺伝的アルゴリズムの実装。 |
| 中村健太郎 | 慶應義塾大学 | 深層学習器の分解再構築 | 深層学習器を構成する各層を独立に実装。連結した状態で手書き数字の分類を行った。さらにこれらのうち任意の一つを選び、新規に構成した深層学習器に組み込み、学習の経過を再利用することが可能か、実装と検証を行った。 |
| 内藤泰宏 | 慶應義塾大学 | Code maintenance of E-Cell 3 | (1) Confirmed that E-Cell 3 can be installed on OS X Yosemite without problem. (2) the first version of ecell3-cellml2eml is committed to the ecell/ecell3 repository. (3) A critical bug of AdaptiveDifferentialStepper was found out (will be fixed very soon). |
| 菊池魁人 | 東京大学 | 1細胞顕微鏡画像データの解析 | 大腸菌の1細胞顕微鏡画像を解析して得られた細胞面積や細胞質中のGFP粒子の座標などのデータを解析し、細胞成長と粒子移動距離を可視化した。 |
| 今井亮輔 | 国立遺伝学研究所 | クロマチンドメインモデルに基づいた、ヌクレオソーム拡散のメトロポリスモンテカルロシミュレーション | クロマチンドメインモデルに基づいて、制限された領域の中でのヌクレオソームの拡散シミュレーションを行った。その結果、培養細胞での観察結果を支持するMSDのパターンが得られた。 |
| chew wei xiang | RIKEN QBiC | Volumetric second-order reaction in Spatiocyte for species with radius &lt; voxel radius. | The reactive collision probability between two volumetric species that undergoes 2nd-order reaction (reversible/ irreversible) are modified such that when radius of species is &lt;= voxel size, correct steady-state behavior are reproduced. |
| 高萩航 | 慶應義塾大学 | whole-ecoliシミュレーションの出力データに対するmicroarray解析ツール””SimuSEQ””の作成 | QBiCで開発中の大腸菌シミュレーションモデル””whole-ecoli””は、出力データをテキストファイルに出力する。このデータをわかりやすく伝えるのは困難である。モデル出力内容を瞬時に、感覚的に理解するツールが存在すれば、外部へのプレゼンや開発者自身のデバッグにも有効であると考え、whole-ecoli出力データに対応したmicroarray解析ツールを作成し、””SimuSEQ””と命名した。SimuSEQは可視化ツールであるが、解析ソフトの側面を持ち、Probe長や位置の変更を簡単に行うことができる上、ユーザが作成したPythonスクリプトにSimuSEQの関数を取り入れることで、データを比較的自由に、しかも簡単に可視化、解析することが可能となった。SimuSEQは、感覚的にわかりにくいミュレーション結果を、まるでwetの実験結果のように、しかも定量的に示すことができる有効なツールであると考えている。 |
| 西田孝三 | RIKEN QBiC | Improving E-Cell4 interoperability with GARUDA | To improve E-Cell4 interoperability, we created two GARUDA gadgets. One gadget is an automatic model generator program, another gadget is E-Cell4 ODE simulator. We showed a pipeline for E-coli metabolic network simulation with these gadgets. This pipeline enables E-Cell4 users to simulate E-coli metabolism just with clicking gadgets. |
| 田中剛貴 | 同志社大学 | リガンドと受容体結合のシミュレーション | 細胞内受容体とそのリガンドの結合をODE-simulatorを用いてE-Cell4上で再現。 |
| 富田　篤弘 | 東京大学 | 細胞内ホメオスタシス維持タンパクと調節因子の生化学シミュレーション | “ecell4のlatticeを利用して細胞内Mg2+ホメオスタシスを維持するタンパクを膜上に構成し、その調節因子とのシミュレーションを行い、調節因子の生理学的役割について考察した。 |
| 森　秀人 | 慶應義塾大学 | Web上でのE-Cellシミュレーション環境の開発 | Webブラウザで実行することのできるE−Cellシミュレーション環境の実装を行った．スプリントでは選択されたモデルファイルを読み込み，その構造をツリー構造としてブラウザに表示することができた． |
| 大竹 悠互 | 慶應義塾大学 | セルオートマトンを用いた膵臓癌のシミュレーション | 本研究である膵臓癌に関する実験の予測や再現をすべく、セルオートマトンを用いたシミュレーションを行うため、Java scriptでライフゲームを作った。 |
| 大沼泰秀 | 慶應義塾大学 | Webbsの出力部分の構築とトップページの作成 | Javascriptを使ってWebbsの出力部分の構築し、またトップページを作成した。出力部分は、シミュレーションの値をダウンロードできるようにした。 |
| 佐々木 啓太 | 慶應義塾大学 | E-Cellを用いたWeb上で実行できるシミュレーションソフトの開発(Webbs) | Web上にて、シミュレーションソフトウェアであるE-Cellを実行できる環境を作成した。サーバー側はPythonを用い、E-Cellの実行を行う。クライアント側はjavascriptを用いてデータの更新、グラフ描画を行う。サーバー、クライアント間のやりとりはNode.js、Websocketを用いて実装を行った。 |
| 板谷 英駿 | 慶應義塾大学 | Integration of cognitive computing platform BriCA and the Robot OS software | The project aimed to implement the functionalites of a BriCA agent object within a ROS Node object to achieve the interoperation of both software. Real-time communication between the two software have been achieved with the use of rospy programming library. |
