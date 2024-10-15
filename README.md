# ICEPP_summercamp2024

本リポジトリは、令和6年度ICEPP量子研究サマーキャンプ<https://www.icepp.s.u-tokyo.ac.jp/collaboration/quantum-summercamp.html>に参加した際に開発したコードを含む。

# 本リポジトリに含まれるコード

* 2値分類問題のための[NTangled Datasets](https://github.com/LSchatzki/NTangled_Datasets?tab=readme-ov-file#ntangled-datasets)を作成するためのコード
* 2値分類問題を解くための量子機械学習モデル[Quantum Convolutional Neural Network](https://www.tensorflow.org/quantum/tutorials/qcnn?hl=ja)のコード

## 2値分類問題のための[NTangled Datasets](https://github.com/LSchatzki/NTangled_Datasets?tab=readme-ov-file#ntangled-datasets)を作成するためのコード

二値分類を行うための教師付き量子データセット[NTangled Datasets](https://github.com/LSchatzki/NTangled_Datasets?tab=readme-ov-file#ntangled-datasets)を作成する。

ランダムな積状態に対し、Ntangled Datasetsのリポジトリ内で示されているパラメータ付き量子回路を作用させることで、特定の[Concentratable Entropy(CE)](https://arxiv.org/abs/2104.06923)（エントロピーの強さを示す指標の一つ）の値を持つエンタングルメント状態を作ることができる。

元のリポジトリでは、3種のパラメータ付き量子回路の構成とそのパラメータの値のみが与えられていた。
そこで、本リポジトリは、3種の量子回路の内、Hardware Efficent(HWE)回路の実装、回路の作用によって作られるエンタングル状態のCEの値の分布の可視化、量子機械学習のためのデータセットの出力を行うコードを含む。

データセットの構成を述べる。

出力データ（ラベル）はランダムな積状態に対し回路を作用させてできるエンタングルメント状態のCEに対応する値である。例として、CE=0.05,0.35のエンタングルメント状態のデータセットならば、データセットファイルに書き込まれる出力データはそれぞれ-1,1となる。

入力データは、積状態を作るためのRZ、RYゲートの回転角と、フラグから成る。


## 2値分類問題を解くための量子機械学習モデル[Quantum Convolutional Neural Network](https://www.tensorflow.org/quantum/tutorials/qcnn?hl=ja)のコード
上で作成したNtangled Datasetsを用いて量子機械学習を行うためのQCNNのコードと、

