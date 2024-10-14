# ICEPP_summercamp2024
令和6年度ICEPP量子研究サマーキャンプ<https://www.icepp.s.u-tokyo.ac.jp/collaboration/quantum-summercamp.html>に参加した際に開発したコード

# 含まれるコード

* [NTangled Datasets](https://github.com/LSchatzki/NTangled_Datasets?tab=readme-ov-file#ntangled-datasets)データセット生成コード
* [Quantum Convolutional Neural Network](https://www.tensorflow.org/quantum/tutorials/qcnn?hl=ja)の実装とNtangled Datasetsの2値分類。

## Ntangled Datasets データセット生成コード
二値分類を行うためのデータセットは、各データは、とそのCEの値に対応するラベルが付与されている。
例として、
[NTangled Datasets](https://github.com/LSchatzki/NTangled_Datasets?tab=readme-ov-file#ntangled-datasets)で紹介されている量子回路とパラメータを使用し、
ランダムな積状態から、特定の[Concentratable Entropy(CE)](https://arxiv.org/abs/2104.06923)（エントロピーの強さを示す指標の一つ）値を持つエンタングルメント状態を作る量子回路

データセットは、

## Ntangled Datasetsを用いた量子機械学習モデル

上で作成したデータセットに対し、二値分類を行うQCNN。


