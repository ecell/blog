+++
date = 2014-10-03T07:00:00Z
lastmod = 2020-05-07T07:00:00Z
author = "Kozo Nishida"
title = "E-Cell sprint 2014を葉山で行いました"
subtitle = ""
feature = ""
+++

今年度のE-Cell sprintを8月31日~9月4日の5日間、神奈川県 葉山 IPC生産性国際交流センターで開催しました。
E-Cell sprintはSystems biology全般に係わるprojectを募り、hackathon形式で開発を行う合宿です。
今年度は参加者がさらに増え(約40名余)、全脳アーキテクチャ関連のprojectも加わり下記のような成果が得られました。
E-Cell sprintは来年も開催する予定ですのでこれらにご興味を持たれた方は[@ktakahashi74](https://twitter.com/ktakahashi74)にお声がけください。

{{< figure src="image/ecell-sprint-2014/screenshot-2014-09-30-20-53-29.png" >}}
{{< figure src="image/ecell-sprint-2014/sprint-2014.jpg" >}}
{{< figure src="image/ecell-sprint-2014/screenshot-2014-09-30-20-57-13.png" >}}
{{< figure src="image/ecell-sprint-2014/screenshot-2014-09-30-20-58-15.png" >}}

## E-Cell4関連
|||||
| -- | -- | -- | -- |
| 加藤傑   | 京大   | Ecell4 LatticeへのStructure実装 | Ecell4に移植したSpatiocyteであるLatticeに細胞膜などの構造体を配置するための下準備として球面上に粒子を配置できるよう拡張 |
| 西田孝三 | 理研   | E-Cell4 rule-base modelの可視化 | E-Cell4のrule-base modelの基本構成単位となるSpeciesをCytoscape.jsを用いcontact mapとして可視化 |
| 海津一成 | 理研   | 空間的GillespieアルゴリズムのE-Cell4上への実装 | 格子と空間均一の中間にあたる空間的Gillespie法の実装 |
| 西田直樹 | 阪大   | Visualizing microbial communities | “Variable Cell Morphology Approach for Individual-Based Modeling of Microbial Communities” (Tomas Storck, DOI: [http://dx.doi.org/10.1016/j.bpj.2014.03.015](http://dx.doi.org/10.1016/j.bpj.2014.03.015))のシミュレータ・ビジュアライザの実装 |
| 坂本裕紀 | 東工大 | Kinetic rate support in ECell4 | E-Cell4における反応速度の定義をUser-definableにhttps://github.com/ecell/ecell4/tree/feature/ratelow |

## Spatiocyte関連
|||||
| -- | -- | -- | -- |
| Satya Arjunan | 理研 | AVX2 SIMD Implementation of Particle Diffusion | The diffusion process of Spatiocyte using Intel Advanced Vector Extensions 2 (AVX2) intrinsics |
| Chin Yin Fai | 理研 | Simulation of Cell Mechanics Reaction Diffutson Model | Testing different parameters or variables on their influence to the PI3K-PTEN wave and how they contribute to the cell protrusion during membrane deformation. |
| 川端政則 岩本一成 | 早稲田 理研 | タンパク質分子の輸送過程のモデル化およびその可視化 | タンパク質分子の合成、細胞膜への輸送、細胞膜上でのラフト形成の 一連の過程をE-Cell3 Spatiocyteにてモデル化、シミュレーション |

## E-Cell3関連
|||||
| -- | -- | -- | -- |
| 内藤泰宏 | 慶応 | E-Cell3 IPython の開発 | ecell3-sessionの機能を IPython で利用可能にする extension を作成。ecell3-sessionが持つ一部の関数に特化したタブ補完機能を実装 |
| 等々力さゆり | 慶応 | 新生児赤血球モデルの構築(赤血球シミュレーション) | 新生児の赤血球で成人型と胎児型のヘモグロビン2種が割合を自由に設定できる形で混在したモデルを構築し、その挙動が正しいか確認 |
| Hitomi Sano 脇田舞子 瀧口真央 | 慶応 | 心筋細胞のコンピュータシミュレーション | cellML2emlの作成と心筋細胞のコンピュータシミュレーション |
| 森秀人 | 慶応 | TNNPモデルのOpenCellからE-Cellへの移植 | OpenCell上で再現されているTNNPモデルをE-Cell上に移植 |
| 山本優理 | 慶応 | 腸内細菌叢シミュレーションプロジェクト-宿主-微生物間相互作用の理解に向けて | Faithらが2011年に発表した数理モデルをE-Cell System、MATLABに移植し，シミュレーションに必要なスクリプトを作成 |

## Systems biology全般
|||||
| -- | -- | -- | -- |
Kaito Kikuchi | 東大 | Creation of a Protein-Protein Interaction Analyzer Garuda Gadget | In the E-Cell Sprint 2014, I made a gadget (application) for the Garuda platform that analyzes protein-protein interaction networks and calculates the statistical significance of the enrichment of a protein group of interest within a given community. The language used was Python 2.7, and the PyQt4 library was used for the GUI.
Soh Ishiguro | 慶応 | Reconstruction of protein complex network for whole cell simulation of E. coli | タンパク質複合体の形成過程をEcocycと呼ばれるデータベースをもとにネットワークとして表現するデータベースの構築 [https://github.com/soh-i/ecellp-ecocyc](https://github.com/soh-i/ecellp-ecocyc)
佐々木啓太 | 慶応 | ロバストネス解析シミュレーションのパッケージ化 | COBRApy内のモジュールを改変し、ロバストネス解析が行うことができるモジュールのパッケージ化
渡部匡己 | 理研 | 生物画像シミュレーション | in-vitro画像とシミュレーション画像の比較
増山七海 | 慶応 | G-languageを用いたCAIとtAIの計算〜組換え遺伝子のコドン最適化にむけて〜 | 大腸菌の高発現遺伝子に対して、任意の塩基配列のCAI値とtAI値を計算するスクリプトの作成

## 全脳アーキテクチャ関連
|||||
| -- | -- | -- | -- |
田中雄一郎 | 慶応 | PS ファイル表現における必要要素の同定スクリプトの作成 | PSファイル表現における,その要素が必要であるのか不必要であるのかを同定するシステムの構築
Satoshi Tamaki | 慶応 | Stacked Denosing AutoEncoderにおけるDeep layerの可視化 | pylearn2を用いたdeep layerの可視化アルゴリズムの実装
Takeshi ITOH | 北大 | Strengthening an Othello AI Using Machine Learning | Developing an AI playing Othello using an evaluation function established by “”Temporal Difference with Monte-Carlo”” [https://github.com/itakeshi/othello.jl&amp;#8221](https://github.com/itakeshi/othello.jl&amp;#8221)
Taku Tsuzuki | 阪大 | Numpyを用いたAutoencoderの実装と、その内部表現の可視化 | Pythonの行列計算モジュールであるNumpyを用いたDeeplearningの手法の一つであるAutoencoderの実装
西田圭吾 | 阪大 | word2vecによる意味区間の形成 | word2vecの意味空間を形成し、学習された各単語の持つ意味空間と自身の直感が一致するかを確認
板谷英駿 | 慶応 | A Naive Implementation of Music Classification using a Recursive Neural Network | コンピュータを用いた音楽の分類を実現するべく機械学習アルゴリズムの有用性を検討
松村直也 | 北大 | 細胞分化に関するダイナミクスのシミュレーション | morphogenの濃度勾配における三つの安定点を持つ系の構築とその数値シミュレーション
