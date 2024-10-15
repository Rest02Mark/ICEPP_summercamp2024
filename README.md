# ICEPP_summercamp2024
本リポジトリは令和6年度ICEPP量子研究サマーキャンプ<https://www.icepp.s.u-tokyo.ac.jp/collaboration/quantum-summercamp.html>に参加した際に開発したコードを含む。

# 本リポジトリに含まれるコード

* 2値分類問題のための[NTangled Datasets](https://github.com/LSchatzki/NTangled_Datasets?tab=readme-ov-file#ntangled-datasets)を作成するためのコード
* 2値分類問題を解くための量子機械学習モデル[Quantum Convolutional Neural Network](https://www.tensorflow.org/quantum/tutorials/qcnn?hl=ja)のコード

## 2値分類問題のための[NTangled Datasets](https://github.com/LSchatzki/NTangled_Datasets?tab=readme-ov-file#ntangled-datasets)を作成するためのコード

二値分類を行うための教師付き量子データセットを作成する。
量子データセットは[NTangled Datasets](https://github.com/LSchatzki/NTangled_Datasets?tab=readme-ov-file#ntangled-datasets)を基に作成する。


例として、
[NTangled Datasets](https://github.com/LSchatzki/NTangled_Datasets?tab=readme-ov-file#ntangled-datasets)で紹介されている量子回路とパラメータを使用し、
ランダムな積状態から、特定の[Concentratable Entropy(CE)](https://arxiv.org/abs/2104.06923)（エントロピーの強さを示す指標の一つ）値を持つエンタングルメント状態を作る量子回路

データセットの構成を述べる。

入力データは、初期状態に対し、ランダムな積状態（）と
出力データ（ラベル）は入力より作られるエンタングルメント状態のCEに対応する値(-1,1)である。

## 2値分類問題を解くための量子機械学習モデル[Quantum Convolutional Neural Network](https://www.tensorflow.org/quantum/tutorials/qcnn?hl=ja)のコード

