# AIによる時系列データ・画像データでの異常検知

- 各[jupyter](https://jupyter.org/)のコードは，[github](https://github.com/hamagami/anomaly-detection)上から[google colab](https://colab.research.google.com/)に読みこむリンクになっています。googleアカウントにログオンしている状態で実行してください。
- サンプルコードは，Cその他の手続き型言語に慣れている方を想定して，必ずしもpythonで推奨される効率的な書き方になっていな部分があります。
- 各コードごとにできるだけ単独で動作させるために，冗長な部分が多々あります。何度も出てくる部分は，ファイルごとに若干書き方が異なる部分がありますが，編集上の都合で実装上の意味はありません。
----------
1. **環境構築**
    1. [テストページ](https://colab.research.google.com/github/hamagami/anomaly-detection/blob/main/00_00_%E7%92%B0%E5%A2%83%E7%A2%BA%E8%AA%8D.ipynb)
2. **異常検知概論**
3. **異常検知のための特徴抽出**
    1. 時系列データの特徴抽出
    2. 画像データの特徴抽出
    3. 距離
        1. [様々な距離](https://colab.research.google.com/github/UsrNameu1/MLStudy/blob/master/VolonoiForMetrics.ipynb) (python2のため外部コード）
        2. [球面集中現象](https://colab.research.google.com/github/hamagami/anomaly-detection/blob/main/%E7%90%83%E9%9D%A2%E9%9B%86%E4%B8%AD%E7%8F%BE%E8%B1%A1.ipynb)
    4. [マハラノビス距離とPCA](https://colab.research.google.com/github/hamagami/anomaly-detection/blob/main/03_04_%E3%83%9E%E3%83%8F%E3%83%A9%E3%83%8E%E3%83%93%E3%82%B9%E8%B7%9D%E9%9B%A2_PCA.ipynb)
    5. [クラスタリング](https://colab.research.google.com/github/hamagami/anomaly-detection/blob/main/03_05_clusteringsample.ipynb)
4. **異常検知のための統計基礎**
    1. [正規分布とカイ二乗分布](https://colab.research.google.com/github/hamagami/anomaly-detection/blob/main/02_01_%E3%82%AB%E3%82%A4%E4%BA%8C%E4%B9%97%E6%A4%9C%E5%AE%9A.ipynb)
    2. 単純ベイズ推定
5. **異常検知アルゴリズム**
    1. [k近傍法](https://colab.research.google.com/github/hamagami/anomaly-detection/blob/main/04_01_knnsample.ipynb)  
    2. [LoF](https://colab.research.google.com/github/hamagami/anomaly-detection/blob/main/04_02_LoF.ipynb) 
    3. [ABOD](https://colab.research.google.com/github/hamagami/anomaly-detection/blob/main/04_03_ABOD.ipynb)
    4. [One class SVM](https://colab.research.google.com/github/hamagami/anomaly-detection/blob/main/04_05_oneclassSVM.ipynb)
    5. [オートエンコーダ](https://colab.research.google.com/github/hamagami/anomaly-detection/blob/main/04_06_AE.ipynb)(AE) *
    6. [VAE](https://colab.research.google.com/github/hamagami/anomaly-detection/blob/main/VAE.ipynb)
    7. [GRU(LSTM)](https://colab.research.google.com/github/SnowMasaya/time_series_anomaly_detect_hands_on/blob/master/advanced/time_series_anomaly_detect_keras.ipynb)　**
    8. [特異値スペクトル](https://colab.research.google.com/github/hamagami/anomaly-detection/blob/main/%E7%89%B9%E7%95%B0%E3%82%B9%E3%83%9A%E3%82%AF%E3%83%88%E3%83%AB.ipynb)
6. **高度な異常検知と応用事例**
    1. [Deep learning](https://colab.research.google.com/github/hamagami/anomaly-detection/blob/main/05_01_CNN.ipynb)　**
    2. [リザバー](https://colab.research.google.com/github/hamagami/anomaly-detection/blob/main/05_02_reservoirad.ipynb) **
    3. [ano-GAN ***](https://github.com/hamagami/anomaly-detection/blob/main/AnoGan_withcont.ipynb) 
    4. [isolation forest](https://colab.research.google.com/github/hamagami/anomaly-detection/blob/main/04_04_isoforestsample.ipynb)
7. 参考（外部サイト）
    1. [PyOd examples(ipynb)](https://colab.research.google.com/github/yzhao062/pyod/blob/master/notebooks/Compare%20All%20Models.ipynb)
    2. [L2 AutoEncoder](https://colab.research.google.com/github/shinmura0/AutoEncoder_vs_MetricLearning/blob/master/L2_vs_Autoencoder.ipynb#scrollTo=LptazVinawMH)　**** 
    3. [Deep Metric Learning](https://github.com/daisukelab/metric_learning/tree/master/MVTecAD)  ****
    4. [異常検知データセット](https://www.mvtec.com/company/research/datasets/mvtec-ad/)
    5. [異常検知ツールキット PyOd](https://pyod.readthedocs.io/en/latest/) 
    

*の数は時間がかかる処理


